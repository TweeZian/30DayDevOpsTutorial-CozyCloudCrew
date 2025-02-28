Day 2 - to create a Game Day Notification Solution

Using
Lambda for serverless code
Simple Notification Service for notifications
Event Bridge for event triggering lambda
IAM for policies and permission control

SNS
Topic creation using Standard
Create subscription

IAM
Create new policy in IAM, using JSON from github https://github.com/ifeanyiro9/game-day-notifications/blob/main/policies/gd_sns_policy.json
Change Resource to match SNS ARN
Create new role with newly created policy and AWSLambdaBasicExecutionRole

Lambda
Create new function w/ Author from scratch
Runtime python
Use existing role, with our newly created role
Get code from git and replace existing
Test code

Event Bridge
Create rule
Set rule type to schedule, and recurring
Use cron expression for finer control of timing {0 9-23/2,0-2/2 * * ? *}
Flexible time window off
Target lambda with created template and empty payload

