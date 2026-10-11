What we'll build
Feature	API endpoint	Purpose
Create a device	POST /devices -- Save a new device
Get all devices	GET /devices	-- Retrieve stored devices
Get one device	GET /devices/{deviceId}	-- Retrieve a specific device

We'll test these endpoints using PowerShell or Postman.
GitHub project structure
We'll organize the repository professionally:
serverless-device-management/
├── src/
│   └── lambda_function.py
├── infrastructure/
│   └── template.yaml
├── tests/
│   └── test_lambda.py
├── events/
│   └── create-device.json
├── .gitignore
├── README.md
└── requirements.txt

We'll use AWS SAM to define and deploy the serverless infrastructure, so your repository includes both the application code and the infrastructure definition.

Our implementation plan
1. Create the project locally — folders, Python Lambda code, and Git repository.
2. Build the Lambda function — validate requests and implement device operations.
3. Define the AWS resources — API Gateway, Lambda, DynamoDB, IAM permissions, and logging.
4. Deploy and test — invoke the API and verify records in DynamoDB.
5. Upload to GitHub — add a clear README, architecture diagram, setup steps, and test examples.
6. Add a DevOps improvement — automate validation and testing with a GitHub Actions workflow.

Cost and security
- We'll start with a minimal architecture and check current AWS pricing and Free Tier eligibility before deployment. Free usage is not guaranteed, and API Gateway, logging, and other services may incur charges.
- We'll use IAM least-privilege permissions rather than administrator access.
- We'll never commit AWS access keys, secret credentials, or environment-specific secrets to GitHub.
- We'll include cleanup instructions so you can delete the deployed resources when finished.
