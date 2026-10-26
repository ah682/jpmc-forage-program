# JPMorgan Chase & Co. Forage coursework

My coursework from the JPMorgan Chase & Co. software engineering virtual experience
on Forage. The repository contains three exercises, their supplied starter code,
patch files and a completion certificate.

## Exercises

- [Task 1](jpmc-task-1-main/): a Python quote-processing client, sample datafeed and
  unit tests.
- [Task 2](jpmc-task-2-main/): a React and TypeScript quote display using Perspective
  and a local Python datafeed.
- [Task 3](jpmc-task-3-main/): a ratio and bounds chart, including the data
  calculations in `DataManipulator.ts`.

## Running the exercises

Each task has its own README and dependency files. For the Python dependencies,
create an environment inside the task directory:

```bash
python3 -m venv .venv
.venv/bin/python -m pip install -r requirements.txt
```

Task 1's `client_test.py` imports `client3`, but the client file is named `client.py`.
That import needs fixing before the tests can run.

Tasks 2 and 3 include npm lockfiles and `start`, `build` and `test` scripts. They use
React 16, `react-scripts` 2 and older Perspective and Puppeteer packages, so running
them with a newer runtime may need dependency updates. The frontend reads the
local datafeed at `http://localhost:8080/query?id=1`.

The original task READMEs and starter code are kept in each exercise directory.
