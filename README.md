Test Plan: 
Dog API Automation Testing
Introduction:
The purpose of this test plan is to outline the strategy, objectives, resources, and schedule for testing the Dog CEO's Dog API. 
This ensures that the API endpoints function as expected and return the correct data.
Test Objectives:
Verify that the API endpoints return the correct status codes.
Ensure the data returned by the endpoints is accurate and in the expected format.
Validate that the endpoints handle invalid inputs gracefully.
Test Environment:
Programming Language: Python
Testing Framework: Pytest
APIs Under Test: DOG CEO

Scenario 1:  Random Dog Image Endpoint
Description: Verify the random dog image endpoint.
Steps:
Send a GET request to https://dog.ceo/api/breeds/image/random.
Verify the status code is 200.
Verify the "status" field is "success".
Verify the "message" field contains a valid URL.
Expected Result: Status code is 200, "status" is "success", and "message" contains a valid URL.
Scenario 2: Breed List Endpoint
Description: Verify the breed list endpoint.
Steps:
Send a GET request to https://dog.ceo/api/breeds/list/all.
Verify the status code is 200.
Verify the "status" field is "success".
Verify the "message" field contains a dictionary of breeds.
Expected Result: Status code is 200, "status" is "success", and "message" contains a dictionary of breeds.
Scenario 3:  Images by Breed Endpoint
Description: Verify the images by breed endpoint.
Steps:
Send a GET request to https://dog.ceo/api/breed/{breed}/images with a valid breed.
Verify the status code is 200.
Verify the "status" field is "success".
Verify the "message" field contains a list of image URLs.
Expected Result: Status code is 200, "status" is "success", and "message" contains a list of image URLs.
Scenario 4: Sub-Breed List Endpoint
Description: Verify the sub-breed list endpoint.
Steps:
Send a GET request to https://dog.ceo/api/breed/{breed}/list with a valid breed.
Verify the status code is 200.
Verify the "status" field is "success".
Verify the "message" field contains a list of sub-breeds.
Expected Result: Status code is 200, "status" is "success", and "message" contains a list of sub-breeds.

Test Execution:
Tests will first be done in Postman for validation.
Develop automated test scripts using Pytest framework to execute the test scenarios outlined above.
Execute the tests against Dog CEO’s APIs.
Monitor test execution results and report any failures or deviations from expected outcomes.



