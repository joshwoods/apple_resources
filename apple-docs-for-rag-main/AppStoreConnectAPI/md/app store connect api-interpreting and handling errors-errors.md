

- App Store Connect API
-  Interpreting and Handling Errors 

API Collection

# Interpreting and Handling Errors

Learn how the App Store Connect API returns errors and handle them in your code.

## Overview

When you send a request to the App Store Connect API, you receive a response that includes an HTTP status code and, in most cases, a response body. To determine your request’s status and handle errors, use the HTTP status code along with the `code` from the ErrorResponse. Interpret the error starting with the most general information first.

### Read the HTTP Status Code

The HTTP status code informs you if the request succeeded or failed. If it succeeded, the HTTP status code is in the 200 range, and the response body contains the requested data. If the request failed, the HTTP status code is in the 400 or 500 range, and the response body contains information about the error. In many cases, the status code may be all you need to properly handle errors. See About the HTTP Status Code for more information.

### Interpret the Error Response

If the API request failed, the ErrorResponse object contains details to help you troubleshoot the error, and a `code` property to use for programmatic error handling. See Parsing the Error Response Code for more information.

### Pinpoint the Source of the Error

In some cases, the error information includes a `source` property that precisely locates the problem in your request. See Pinpointing the Location of Errors for more information.

## Topics

### Handling Errors

About the HTTP Status Code

Learn how the status code helps you determine if an App Store Connect API request succeeded or why it failed.

Parsing the Error Response Code

Interpret the error details to troubleshoot API requests and perform programmatic error handling.

Pinpointing the Location of Errors

Locate the specific source of the error.

### Objects

object ErrorLinks

object ErrorResponse

The error details that an API returns in the response body whenever the API request isn’t successful.

