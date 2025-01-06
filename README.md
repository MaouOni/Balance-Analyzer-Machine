# Balance-Analyzer-Machine
Balance Analyzer Machine has the purpose to obtain information from a csv balance document, such as larger amount movement, minor amount movement, banking balance categorization and percentiles based on amount.
It is built on NodeJS and deployed with AWS.
For users authentication is using Cognito, then redirects to a Cloudfront S3 bucket where frontend is located.
Once the user is logged in, will be able to select a csv balance file and subsequently the Balance Analyzer Machine brings back
the next information:
* Larger and minor amount
* Percentil analysis
* Balance categoritzation
Except for categorization, logic programmed on backend performs all the tasks, however can not categorize what type of balance
is on the csv file. Therefore the implentation for this task is performed by a LM.
