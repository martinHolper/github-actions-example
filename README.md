This is setting up a CI/CD Pipline with github actions following: https://youtu.be/NppkHKvnrqc?si=MrX0RFVHB5fvQCe-

all Actions findable under:  https://github.com/actions 
e.g. checkout
https://github.com/actions/checkout
To find out exactly what happens see .yml files under https://github.com/actions/checkout/tree/main/.github/workflows


We use the following steps currently:

    Checkout
    actions/checkout@v4

    Setup Java
    actions/setup-java@v4


Common Errors and Fixes:

Error:

Error: HTTP Status 403 for request POST https://api.github.com/repos/martinHolper/github-actions-example/dependency-graph/snapshots
Error: Response body:
{
  "message": "Resource not accessible by integration",


Fix:
https://github.com/martinHolper/github-actions-example/settings/actions set 

Workflow permissions

Read and write permissions

