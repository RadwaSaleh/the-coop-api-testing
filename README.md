# the-coop-api-testing
REST APIs tests using postman for [The Coop](http://coop.apps.symfonycasts.com/api) APIs.


#### Dependencies
- NodeJS
- newman `npm install -g newman`
- newman-html-reporter `npm install -g newman-reporter-html`


#### Run Tests on Postman
1. Download The_Coop_API.postman_collection.json file
2. Open postman to view and run tests:

Import > File > Choose Files > Select The_Coop_API.postman_collection.json

#### Run Tests with CLI
1. Download the `The_Coop_API.postman_collection.json` file 
2. No need to download the environment file as the token has expiration time and will be generated and saved as environment variable. Only use the same file name or exchange it in the following command
`newman run The_Coop_API.postman_collection.json -e Dev_The_Coop.postman_environment.json -r html`
3. This will create a directory "newman" that will contain html report 

#### Expected Results 
All passing except 3 failed tests with prefix "INTENDED FAILURE"
TODO: Report the 3 issues in [Issues tab](https://github.com/RadwaSaleh/the-coop-api-testing/issues)
![alt text](https://github.com/RadwaSaleh/the-coop-api-testing/blob/main/newman/newman%20report%20example.png)
