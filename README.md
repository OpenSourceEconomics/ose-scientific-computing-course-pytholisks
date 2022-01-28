# Summary of OSE Scientific Computing Project on `pydsge` (by Yuxin, Altaf and Philipp)
---
![Continuous Integration](https://img.shields.io/github/workflow/status/OpenSourceEconomics/ose-scientific-computing-course-pytholisks/Continuous%20Integration%20Workflow?label=Continuous%20Integration&logo=github)

## Testing with pytest
 - A testing suite for regression testing of the tutorial(s) was created
 - A preliminary test against a closed form solution of a smaller model was created
 - A basic test of the parser was created
## Multiprocessing on Windows
 - A pull-request with the relevant changes was created for grglib
 - Gregor’s simplifications were adopted
 - for documentation purposes and Prof. Eisenhauer, full details are provided in [Summary.pdf](https://docs.google.com/document/d/1kWifKdqk_KpfPecELgSkH08Cj23xyQV2hYSu_m4Rjg0/edit?usp=sharing)
## Estimation Tutorial
 - An estimation tutorial for pydsge was created based on a script provided by Gregor
 - Several issues that were discovered in the process were fixed, documentation was improved
## Pre-commit check of Code style
 - A pre-commit hook was created which, among others, includes black, blacken and flake8 (with several adjustments)
## Continuous Integration Workflow
 - To enable cross-platform and cross-version code control and maintenance, a github CI workflow for Unix, MacOs and Windows as well as Python 3.8 and 3.9 was created. (Having a specific  badge for these environments would require Anaconda)
 - The CI workflow runs the pytest framework and, if needed, can be set to update the pickle used for the tests (Ubuntu with python 3.8 is used as the stable version.)

