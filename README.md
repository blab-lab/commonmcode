# This repository is being prepared for archiving.
As of Summer 2026, it is not recommended to use this repository. If you were only using this repository for compatibility with the blab-lab fork of Audapter or other SMNG software, you no longer need it. You can remove the commonmcode repository from your MATLAB path, move it to the bottom of your MATLAB path, or just delete the commonmcode folder entirely.

# About the commonmcode repository
This repository was authored by Shanqing Cai (shanqing.cai@gmail.com; github.com/shanqing-cai/commonmcode). This fork (github.com/blab-lab/commonmcode) was used by the Speech Motor Neuroscience Group (SMNG) at UW-Madison until Summer 2026, but we will not be using the repository or updating it going forward. A small number of functions from this repository, less than 5%, were copied into the blab-lab/audapter_matlab repository if Audapter relied on them, or copied into the carrien/free-speech repository if SMNG code referenced those functions.

# Recommendations for collaborators of the Speech Motor Neuroscience Group
If you previously used this repository, it was probably because you used our group's version of Audapter (github.com/blab-lab/audapter_mex). You should do these steps either now, or the next time you update your Audapter-related repositories:
1. Pull updates to blab-lab/audapter_matlab repository, which is a required repository for using the SMNG version of Audapter.
2. If you were only using the commonmcode repository for compatibility with the blab-lab fork of Audapter or other SMNG software, you no longer need it. You can remove the commonmcode repository from your MATLAB path, move it to the bottom of your MATLAB path, or just delete the commonmcode folder entirely.
3. If you use the carrien/free-speech repository, pull updates to that repository.

# Why are we making this change?
The commonmcode repository contained a lot of functions that were not useful to our lab. Also, MATLAB had released built-in functions, often as one-liners, which performed the same utility as functions in commonmcode. In other cases, commonmcode functions used the same name as other functions we used, which made it hard to know which function was the "real" one.

These problems were all solved by bringing the handful of relevant commonmcode functions into the blab-lab/audapter_mex repository, which everyone running the blab-lab fork of Audapter need anyway. Now there is one less repository that collaborators need to use, and there are fewer duplicate functions.

# Points of contact
For questions/issues, contact Chris Naber (cwnaber@wisc.edu) and Carrie Niziolek (cniziolek@wisc.edu).
