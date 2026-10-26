# JPMorgan Chase & Co. Forage coursework

Historical learning material from the JPMorgan Chase & Co. software engineering
virtual experience on Forage. These directories retain supplied task starters,
course exercises, patch files and a completion certificate. They represent
coursework, not employment at JPMorgan Chase, client delivery or an independently
authored trading platform.

## Contents

- `jpmc-task-1-main/`: Python quote-processing client, sample data, server and unit
  test exercise. The checked-in test imports `client3`, while the supplied file is
  `client.py`; this legacy mismatch must be resolved deliberately before claiming
  a working test run.
- `jpmc-task-2-main/`: React/TypeScript quote display with Perspective integration
  and a local Python datafeed.
- `jpmc-task-3-main/`: React/TypeScript ratio/bounds visualization exercise, including
  `DataManipulator.ts` and the Perspective graph.

## Revisit locally

Read the README and dependency files inside each task before running it. Task 1's
listed Python dependency is `python-dateutil`; a local environment can be prepared
with `python3 -m venv .venv` and `python -m pip install -r requirements.txt` from
that task directory. Its current test-file mismatch is documented above, not
silently represented as passing.

Tasks 2/3 include npm lockfiles and `start`, `build`, `test` scripts. They use legacy
React 16, `react-scripts` 2, older Perspective packages and Puppeteer. Review their
runtime/package compatibility before installing; this repository is not a maintained
production template. The frontend datafeed URL is `http://localhost:8080/query?id=1`;
no real market feed or brokerage is integrated here.

This documentation update has not established a clean modern install or rerun the
course environment. Keep changes attributable: identify supplied scaffolding,
exercise modifications and any later maintenance separately. JPMorgan Chase,
Forage and library names/materials retain their respective owners' rights. A course
completion certificate does not grant reuse rights or imply endorsement. No new
licence is granted by this README.
