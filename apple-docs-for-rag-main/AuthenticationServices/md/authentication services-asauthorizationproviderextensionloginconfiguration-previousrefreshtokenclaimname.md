

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  previousRefreshTokenClaimName 

Instance Property

# previousRefreshTokenClaimName

The claim name for the previous single sign-on token value in the authentication request.

macOS 13.0+

``` source
var previousRefreshTokenClaimName: String { get set }
```

## Mentioned in 

Creating and validating a login request

## See Also

### Configuring the previous refresh token

var includePreviousRefreshTokenInLoginRequest: Bool

A Boolean value that indicates whether to include the previous refresh token in the authentation request.

