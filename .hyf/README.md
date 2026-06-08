# Auto grade tool

## How it works
1. The auto grade tool runs the `test.sh` script located in this directory.
2. `test.sh` should write to a file named `score.json` with following JSON format:
   ```json
   {
     "score": <number>,
     "passingScore": <number>,
     "pass": "<boolean>"
   }
   ```
   All scores are out of 100. It is up to the assignment to determine how to calculate the score.
3. The auto grade runs via a github action on PR creation and updates the PR with the score.

