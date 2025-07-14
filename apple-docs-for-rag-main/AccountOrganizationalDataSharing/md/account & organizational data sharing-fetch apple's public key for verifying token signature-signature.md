

- Account &amp; Organizational Data Sharing
-  Fetch Apple's public key for verifying token signature 

Web Endpoint

# Fetch Apple's public key for verifying token signature

Retrieve the public key associated with the cryptographic identity Apple uses to sign the token.

AccountOrganizationalDataSharing 1.0+

## URL

``` source
GET https://appleid.apple.com/auth/oauth2/v2/keys
```

## Response Codes

` 200 ``OK`

JWKSet

`OK`

The request was successful.

Content-Type: application/json

## Overview

If successful, the HTTP status code is 200 (OK), and the JWKSet.Keys object contains Apple’s public key.

## See Also

### Generating tokens

Creating a client secret

Generate a signed token to identify your client application.

Generate and validate tokens

Validate an authorization grant code delivered to your app to obtain tokens, or validate an existing refresh token.

