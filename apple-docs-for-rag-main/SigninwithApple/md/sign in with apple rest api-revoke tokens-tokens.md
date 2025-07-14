

- Sign in with Apple REST API
-  Revoke tokens 

Web Service Endpoint

# Revoke tokens

Invalidate the tokens and associated user authorizations for a user when they are no longer associated with your app.

Sign in with Apple REST API 1.0+

## URL

``` source
POST https://appleid.apple.com/auth/revoke
```

## HTTP Body

`form-data`

The list of input parameters required for the server to invalidate the token.

Content-Type: application/x-www-form-urlencoded

### Parts

`client_id`

`string`

(Required) 

The identifier (App ID or Services ID) for your app. The identifier must match the value provided during the authorization request for the user’s information. Additionally, the identifier must not include your Team ID, to help mitigate the possibility of exposing sensitive data to the end user.

`client_secret`

`string`

(Required) 

A secret JSON Web Token (JWT) that uses the Sign in with Apple private key associated with your developer account. For more information about creating client secrets, see Creating a client secret.

`token`

`string`

(Required) 

The user refresh token or access token intended to be revoked. The user session associated with the token provided is revoked if the request is successful.

`token_type_hint`

`string`

A hint about the type of the token submitted for revocation. Use `refresh_token` or `access_token`.

## Response Codes

` 200 ``OK`

`OK`

The request was successful; the provided token has been revoked successfully or was previously invalid.

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

The server was unable to process the request. See the error code description for more information about the underlying error.

Content-Type: application/json

## Discussion

In order to revoke authorization for a user, you must obtain a valid refresh token or access token. If you don’t have either token for the user, you can generate tokens when validating an authorization code. For more information about user tokens and creating client secrets, see Generate and validate tokens.

To invalidate a user’s refresh token, invoke the revoke endpoint with the following HTTP POST method.

```
curl -v POST "https://appleid.apple.com/auth/revoke" \
-H 'content-type: application/x-www-form-urlencoded' \
-d 'client_id=CLIENT_ID' \
-d 'client_secret=CLIENT_SECRET' \
-d 'token=REFRESH_TOKEN' \
-d 'token_type_hint=refresh_token'
```

Additionally, to invalidate a user’s access token, use the following HTTP POST method.

```
curl -v POST "https://appleid.apple.com/auth/revoke" \
-H 'content-type: application/x-www-form-urlencoded' \
-d 'client_id=CLIENT_ID' \
-d 'client_secret=CLIENT_SECRET' \
-d 'token=ACCESS_TOKEN' \
-d 'token_type_hint=access_token'
```

For either token revocation request, the `revoke` endpoint returns a `200` response code without a response body after the server invalidates the `token` value, or if the `token` value was previously invalidated. If the response contains an error, please see ErrorResponse for the specific error code provided in the response body.

## See Also

### Generating and revoking tokens

Creating a client secret

Generate a signed token to identify your client application.

Fetch Apple’s public key for verifying token signature

Fetch Apple’s public key to verify the ID token signature.

Generate and validate tokens

Validate an authorization grant code delivered to your app to obtain tokens, or validate an existing refresh token.

