

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  tokenEndpointURL 

Instance Property

# tokenEndpointURL

The token endpoint URL for login requests.

macOS 13.0+

``` source
var tokenEndpointURL: URL { get set }
```

## Mentioned in 

Creating and validating a login request

Creating a refresh request

## See Also

### Obtaining the required configuration

var audience: String

The audience for validation and requests.

var clientID: String

The identifier for the client at the identity provider.

var jwksEndpointURL: URL

The JSON Web Key Set endpoint URL for keys.

var issuer: String

The issuer of the identity token that the identity provider returns.

