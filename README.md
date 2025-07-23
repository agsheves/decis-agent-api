** This is a work in progress **

# Decis Agents API

Decis users can access the agents and other Decis functions via an API endpoint. This is designed to act as a turn- or function-based programmatic interface for request and is different from the [country data API](https://github.com/agsheves/Decis-Country-Data-API/blob/main/README.md), which creates a data feed.

# Quickstart

(You will need your Decis username and password)

## 1 - Create a set of session credentials

Initiate the session
```
code snippet
```

The response will include a ```sessin_id``` and ```access_token```

## 2 - Use the session credentials in the request header to send a query to the agent. The request format is as follows:

* Authentication
* Query
* Tools (including)
  * Country info
  * Risk manager
  * Scenario
 
(*Note: specifying a tool in the query bypasses the Decis orchestration so the tool selection must exactly match the available tools to avoid an error*)

Example

```
code example here

response here
```

The ```session_id``` is the permanent UUID for that session to allow future access, but the ```access_token``` is non-persistent and expires after XX time to preserve session security. Reauthentication with the username/password is necessary to access a session once the access_token has expired.

# 
