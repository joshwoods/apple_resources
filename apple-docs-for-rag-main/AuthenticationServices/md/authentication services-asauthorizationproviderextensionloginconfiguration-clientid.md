

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  clientID 

Instance Property

# clientID

The identifier for the client at the identity provider.

macOS 13.0+

``` source
var clientID: String { get }
```

## Mentioned in 

Processing the JSON Web Encryption (JWE) login response

Creating and validating a login request

Supporting key requests and key exchange requests

Creating a refresh request

## See Also

### Obtaining the required configuration

var audience: String

The audience for validation and requests.

var jwksEndpointURL: URL

The JSON Web Key Set endpoint URL for keys.

var tokenEndpointURL: URL

The token endpoint URL for login requests.

var issuer: String

The issuer of the identity token that the identity provider returns.

