# About the commonmcode repository
This repository was authored by Shanqing Cai (shanqing.cai@gmail.com; github.com/shanqing-cai/commonmcode). This fork (github.com/blab-lab/commonmcode) was used by the Speech Motor Neuroscience Group (SMNG) at UW-Madison until Summer 2026, but we will not be using the repository or updating it going forward. A small number of functions from this repository, about 5%, were copied into the carrien/free-speech repository if other SMNG code referenced those functions.

# Recommendations for collaborators of the Speech Motor Neuroscience Group
If you previously used this repository, it was probably because you used our group's version of Audapter (github.com/blab-lab/audapter_mex). You should do these steps either now, or the next time you update your Audapter-related repositories:
1. Pull updates to the carrien/free-speech repository and the blab-lab/audapter_matlab repository. These are required repositories for using the SMNG version of Audapter.
2. If you were only using the commonmcode repository for compatibility with SMNG software, either remove the commonmcode repository from your MATLAB path or just delete the commonmcode folder entirely.
3. Update the Audapter.mexw64 file to version b2.5. More detailed steps are in that repository's README: github.com/blab-lab/audapter_mex. Until you do this step, you will see warnings when you initialize Audapter.

# Why are we making this change?
The commonmcode repository contained a lot of functions that were not useful to our lab. Also, MATLAB had released built-in functions, often as one-liners, which performed the same utility as functions in commonmcode. In other cases, commonmcode functions used the same name as other functions we used, which made it hard to know which function was the "real" one.

These problems were all solved by bringing only relevant commonmcode functions into the carrien/free-speech repository, which all SMNG collaborators need anyway. Now there is one less repository that collaborators need to use, and there are fewer duplicate functions.

# Points of contact
For questions/issues, contact Chris Naber (cwnaber@wisc.edu) and Carrie Niziolek (cniziolek@wisc.edu).
