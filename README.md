# VulDeeLocator: Deep Learning-based Vulnerability Detection Leveraging Intermediate Code and Granularity Refinement


We propose Vulnerability Deep learning-based Detector and Locator (VulDeeLocator), which is the first deep learning-based vulnerability detector that can simultaneously achieve a high detection capability and a high locating precision. The core innovations underlying VulDeeLocator are (i) the leverage of intermediate code to accommodate semantic information that cannot be conveyed by source code, and (ii) the concept of granularity refinement for precisely pinning down locations of vulnerabilities.

We extract pieces of source code according to some syntax information (i.e., source code- and Syntax-based Vulnerability Candidate or sSyVC for short), involving four kinds of sSyVCs: library/API function call (FC), array definition (AD), pointer definition (PD), and arithmetic expression (AE). Then we extend these pieces of code to accommodate the semantic information from the intermediate code (i.e., intermediate code- and Semantics-based Vulnerability Candidate or iSeVC for short).

We prepare a dataset of Lower Level Virtual Machine (LLVM) intermediate code from two data sources: the National Vulnerability Database (NVD) and the Software Assurance Reference Dataset (SARD). It involves 10,246 training programs and 2,561 target programs. The resulting dataset contains 159,102 vulnerability candidates in intermediate code (i.e., iSeVC), among which 37,293 are vulnerable and 121,809 are not vulnerable. We provide the dataset for training purpose and testing purpose for each kind of sSyVC respectively. For vulnerable iSeVCs, the line numbers of the vulnerabilities are available. 
