

- Sign in with Apple REST API
-  TokenResponse 

Object

# TokenResponse

The response token object returned on a successful request.

Sign in with Apple REST API 1.0+

``` source
object TokenResponse
```

## Properties

`access_token`

`string`

A token used to access allowed data, such as generating and exchanging transfer identifiers during user migration. For more information, see Transferring your apps and users to another team and Bringing new apps and users into your team.

`expires_in`

`number`

The amount of time, in seconds, before the access token expires.

`id_token`

`string`

A JSON Web Token (JWT) that contains the user’s identity information.

`refresh_token`

`string`

The refresh token used to regenerate new access tokens when validating an authorization code. Store this token securely on your server. The refresh token isn’t returned when validating an existing refresh token.

`token_type`

`string`

The type of access token, which is always `bearer`.

## See Also

### Common objects

object JWKSet

A set of JSON Web Key objects.

object ErrorResponse

The error object returned after an unsuccessful request.

