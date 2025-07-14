

- Authentication Services
- Platform single sign-on (SSO)
- Authentication process
-  Obtaining a server nonce 

Article

# Obtaining a server nonce

Request and process a server nonce to verify communication and detect replays.

## Overview

The login request, refresh request, and key requests use the server nonce so the identity provider (IdP) can verify it’s communicating to a live client. The IdP can also use the server nonce for replay detection.

### Create the server nonce network request

The following table specifies the header parameters that the system uses to create a server nonce request:

| Key | Value | Notes |
|----|----|----|
| `grant_type` | `srv_challenge` | Required. |
| customNonceRequestValues |  | Optional. If present, adds the key value pairs to the request. |
| `client-request-id` | `UUID` | Required. A unique identifier for the request. |

The server nonce request is an HTTP POST to the login configuration nonceEndpointURL, as shown in the following example:

```
```

### Receive the server nonce network response

If the http status is `200`, the response body loads as JSON. If the body is valid JSON, the system pulls the server nonce from the response using the login configuration nonceResponseKeypath or the default value `Nonce`.

Platform SSO doesn’t validate the token and treats it as an opaque value.

## See Also

### Pre-login

Performing a preauthentication request

Request and process a preauthentication for dynamic WS-Trust authentication.

Performing a WS-Trust metadata exchange data (MEX) request

Send and process a WS-Trust MEX request to determine the version and URLs for authentication.

