

- Apple Search Ads
-  Calling the Apple Search Ads API 

API Collection

# Calling the Apple Search Ads API

Pass your access token in the authorization header of HTTP requests.

## Overview

Before you can call the API, you need to perform the implementation steps in Implementing OAuth for the Apple Search Ads API.

To call the Apple Search Ads Campaign Management API, pass your access token as `Bearer` in the authorization header of HTTP requests. The `Bearer` value informs the API that the bearer of the token has authorization to access the API and perform specified actions. The following is an example call to the API:

```
```

| **Header** | **Description** |
|----|----|
| `Authorization` | **Required**. The authorization value is always `Bearer`. |
| `X-AP-Context` | **Required**. The value is your `orgId`.  **Note**: This isn’t a requirement when calling Get User ACL and Get Me Details. |

To return the `userId` and `parentOrgId` of an API caller, use Get Me Details.

### Handle Errors

| **HTTP status code** | **Error message** | **Description** |
|----|----|----|
| `401` | `unauthorized` | The token is invalid or expired. |
| `403` | `forbidden` | The request requires higher privileges than the access token provides. |

### Rate Limits

Rate limits exist in the Apple Search Ads Campaign Management API to avoid latency and other system problems from too many API calls within a limited time. For API users that are using automated retry logic in their environments, Apple’s solution is to require the retry logic to increase retry attempts exponentially by seconds. For example, if your default minimum wait time between retries is 2 seconds, the next retry wait time is 4 seconds, and so forth.

Set a maximum exponential backoff time, such as 16 seconds. After reaching the maximum time, don’t increase the wait period between retries.

- If the request fails, wait 2 seconds and retry the request.

- If the request fails, wait 4 seconds and retry the request.

- If the request fails, wait 8 seconds and retry the request.

- If the request fails, wait 16 seconds and retry the request.

## Topics

### Access Control List

Get User ACL

Fetches roles and organizations that the API has access to.

object UserAcl

The response to ACL requests.

object UserAclListResponse

A container for ACL call responses.

Get Me Details

Fetches details of an API caller.

object MeDetail

The API caller identifiers.

object MeDetailResponse

The response from me detail calls.

### Error Responses

object ApiErrorResponse

A parent object of the error response body.

object ErrorResponseBody

A parent object of the error response.

object ErrorResponseItem

The error response details in the response body.

object IntegerResponse

A common integer type response.

object VoidResponse

A default generic null response.

## See Also

### Essentials

Implementing OAuth for the Apple Search Ads API

Manage secure access to Search Ads accounts.

Using Apple Search Ads API Functionality

Call endpoints using CRUD methods.

