# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Role profiles, course catalogues and results, scored as they arrive |
| SageMaker AI | Gap ranking and course matching per role |
| Bedrock | Pathway explanations a manager can read in a minute |
| DynamoDB | People, skills, pathways and the approval log |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
