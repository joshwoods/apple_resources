

- Sign in with Apple REST API
-  Fetch Apple’s public key for verifying token signature 

Web Service Endpoint

# Fetch Apple’s public key for verifying token signature

Fetch Apple’s public key to verify the ID token signature.

Sign in with Apple REST API 1.0+

## URL

``` source
GET https://appleid.apple.com/auth/keys
```

## Response Codes

` 200 ``OK`

JWKSet

`OK`

The request was successful.

Content-Type: application/json

## Mentioned in 

Processing changes for Sign in with Apple accounts

## Discussion

If successful, the HTTP status code is 200 (OK) and the JWKSet.Keys object contains Apple’s public key

Note

The endpoint can return multiple keys, and the count of keys can vary over time. From this set of keys, select the key with the matching key identifier (`kid`) to verify the signature of any JSON Web Token (JWT) issued by Apple. For more information, see the JSON Web Signature specification.

## See Also

### Generating and revoking tokens

Creating a client secret

Generate a signed token to identify your client application.

Generate and validate tokens

Validate an authorization grant code delivered to your app to obtain tokens, or validate an existing refresh token.

Revoke tokens

Invalidate the tokens and associated user authorizations for a user when they are no longer associated with your app.

