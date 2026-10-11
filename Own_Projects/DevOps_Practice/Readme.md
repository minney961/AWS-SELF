                  AWS PLATFORM ENGINEER
                           |
          +----------------+----------------+
          |                |                |
       IaC              Serverless       Security
          |                |                |
       CDK             Lambda          IAM
    TypeScript       API Gateway        KMS
   CloudFormation     DynamoDB       Secrets Manager
          |                |                |
          +----------------+----------------+
                           |
                  Event Driven Architecture
                           |
                     +-----+-----+
                     |           |
                    SQS      EventBridge
                     |
                  Lambda
                     |
                 DynamoDB/S3
                           |
                  +--------+--------+
                  |                 |
              CloudWatch          X-Ray
                  |
              Monitoring
