

- Advanced Commerce API
-  Authorizing API requests from your server 

Article

# Authorizing API requests from your server

Create JSON Web Tokens (JWTs) to authorize Advanced Commerce requests from your server.

## Discussion

The following Advanced Commerce APIs are endpoints that you call from your server:

- Cancel a Subscription

- Change Subscription Metadata

- Change Subscription Price

- Migrate a Subscription to Advanced Commerce API

- Request Transaction Refund

- Revoke Subscription

Calls to the Advanced Commerce API’s endpoints require JSON Web Tokens (JWTs) for authorization; you obtain keys to create the tokens from your organization’s App Store Connect account. See Creating API keys to authorize API requests to create your keys. See Generating JSON Web Tokens for API requests to generate tokens using your keys and send API requests.

After you have a complete and signed token, provide the token in the request’s authorization header as a bearer token. Generate a new token for each new API request, or reuse tokens until they expire.

Tip

The App Store Server Library provides a client that makes it easier to adopt the Advanced Commerce APIs, including creating the JWTs to authorize calls. For more information, see Simplifying your implementation by using the App Store Server Library.

## See Also

### API authorization and rate limits

Identifying rate limits for Advanced Commerce APIs

Recognize and handle the rate limits that apply to Advanced Commerce API endpoints.

