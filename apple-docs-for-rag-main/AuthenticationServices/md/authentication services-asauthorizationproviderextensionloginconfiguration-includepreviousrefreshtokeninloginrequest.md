

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  includePreviousRefreshTokenInLoginRequest 

Instance Property

# includePreviousRefreshTokenInLoginRequest

A Boolean value that indicates whether to include the previous refresh token in the authentation request.

macOS 13.0+

``` source
var includePreviousRefreshTokenInLoginRequest: Bool { get set }
```

## Mentioned in 

Creating and validating a login request

## Discussion

If the value is `true` and there’s a `refresh_token` for the user in the SSO tokens, it’s included in the authentication request.

## See Also

### Configuring the previous refresh token

var previousRefreshTokenClaimName: String

The claim name for the previous single sign-on token value in the authentication request.

