

- Advanced Commerce API
-  Identifying rate limits for Advanced Commerce APIs 

Article

# Identifying rate limits for Advanced Commerce APIs

Recognize and handle the rate limits that apply to Advanced Commerce API endpoints.

## Overview

The Advanced Commerce API limits the number of requests that you can submit to each endpoint within a specified timespan. The request limits apply per app. The following table lists the rate limits in the production environment, expressed in requests per second. Limits are enforced on an hourly basis.

| Endpoint | Rate limit (per second) |
|----|----|
| Cancel a Subscription | 5 |
| Change Subscription Metadata | 50 |
| Change Subscription Price | 50 |
| Migrate a Subscription to Advanced Commerce API | 50 |
| Request Transaction Refund | 5 |
| Revoke Subscription | 5 |

The rate limits in the sandbox environment are 10 percent of the limits in the table above. The Advanced Commerce server may make adjustments to reduce or increase these rate limits as needed at any time.

### Handle exceeded rate limits gracefully

If you exceed a per-hour limit, the API rejects the request with an `HTTP 429` response, with a RateLimitExceededError in the body. Consider the following as you integrate the API:

- If you periodically call the API, throttle your requests to avoid exceeding the per-hour limit for an endpoint.

- Manage the `HTTP 429 RateLimitExceededError` in your error-handling process. For example, log the failure and queue the job to process it again at a later time.

- Check the `Retry-After` header if you receive the `HTTP 429` error. This header contains a UNIX time, in milliseconds, that informs you when you can next send a request.

## See Also

### API authorization and rate limits

Authorizing API requests from your server

Create JSON Web Tokens (JWTs) to authorize Advanced Commerce requests from your server.

