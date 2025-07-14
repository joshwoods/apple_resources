

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  audience 

Instance Property

# audience

The audience for validation and requests.

macOS 13.0+

``` source
var audience: String { get set }
```

## Mentioned in 

Supporting key requests and key exchange requests

Creating an embedded assertion

Creating an encrypted embedded assertion

## See Also

### Obtaining the required configuration

var clientID: String

The identifier for the client at the identity provider.

var jwksEndpointURL: URL

The JSON Web Key Set endpoint URL for keys.

var tokenEndpointURL: URL

The token endpoint URL for login requests.

var issuer: String

The issuer of the identity token that the identity provider returns.

