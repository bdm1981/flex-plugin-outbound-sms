# Outbound Initiated SMS

This plugin allows Twilio Flex agents to initiate an outbound converations. The plugin works leverages several Twilio Functions to orchestrate creating a new task.

![Componenet Screenshot](/screenshots/outbound-component.png?raw=true "Componenet Screenshot")

## Prerequisites

1. Install the Flex Plugin for Twilio CLI. [Instructions](https://www.twilio.com/docs/flex/developer/plugins/cli/install)

## Setup

1. copy or rename the .env_sample to .env. 
1. Set the FLEX_APP_FUNCTIONS_URL to the Serverless Runtime domain that is hosting the support Twilio Functions

## Deploy

Run the following command
```bash
twilio flex:plugins:deploy --major --changelog "Notes for this version" --description "Functionality of the plugin" 
```

Once deployed run the following command to release the command
```bash
twilio flex:plugins:release --plugin example-plugin@1.0.0 --plugin additional-plugin@2.1.0 --name "Example 1" --description "Demonstrating use of twilio flex:plugins:release"
```