# performance-testing with Artillery.io

Setup instructions:

  1. Clone the repository and run `npm i` in the root of the project folder
  2. Add configurations for your website in a configuration file in the tests/configs folder.
  3. Add test scenarios (Build scenarios to load test various endpoints) to the tests/scenarios folder.
  4. Run the scenario script with the configuration. 
  Example : 
  The command to run is `artillery run --config ./tests/configs/test-app-config.yml ./tests/scenarios/outsmart-dispensary-actions.yml --output sample.json`
  * The --config hook specifies the config file which is followed by the scenario file. The --output hook specifies the test output which will be a json file.
  
  5. Generate an html report with the command: `artillery report --output sample.html sample.json`
  * The --output command specifies the name of the html reports followed by the json file generated from the previous run command.
  
  The html report can then be opened in the browser. Reports are stored in the root of the project. Sample outputs can be found in the reports folder.
  
  Helpful Resources:
  - https://www.artillery.io/docs
  - https://www.artillery.io/docs/guides/getting-started/writing-your-first-test
  - https://www.artillery.io/docs/guides/getting-started/core-concepts
  - https://www.artillery.io/docs/guides/guides/http-reference
  
