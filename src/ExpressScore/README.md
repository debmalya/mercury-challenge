# ExpressScorer
**ExpressScorer** is a lightweight scoring application that does not require a Docker installation.  It only performs minimal input validation and it does not compute lead times.

- Documentation:  https://github.com/planetmercury/mercury-challenge/tree/master/src/ExpressScore/notebooks
- Dependencies:  See <https://github.com/planetmercury/mercury-challenge/blob/master/src/ExpressScore/expressscore.yml> for a minimal Anaconda enviroment that will run the code under Python 3.4.  Please note that VisualStudio tools may be necessary to build and run this on Windows.
- Usage:
  - *MaScorer*
    - `from express_score import MaScorer`
    - `scorer = MaScorer(country)`
    - `scorer.score(warn_data, gsr_data)`
  - *CaseCountScorer*
    - `from express_score import CaseCountScorer`
    - `scorer = CaseCountScorer(event_type, location)`
    - `scorer.score(warn_data, gsr_data)`
- Unittests (run from https://github.com/planetmercury/mercury-challenge/tree/master/src/ExpressScore/test)
  - `python test_case_count_scorer.py`
  - `python test_ma_scorer.py`

All code in this package is provided using the CC0 1.0 Universal (CC0 1.0) Public Domain Dedication.
