# SQS, CloudWatch Alarms, and Slack

This repo is an example of how to do 3 things:

-   Setup a DLQ so you wll never lose SQS messages that are unable to be processed. This can happen when there are bugs in the code, the input is not formatted correctly, or there is a service outage.
-   How to setup a CloudWatch alarm when any unprocessed messages appear in the DLQ
-   How to notify a Slack channel whenever this alarm is triggered
