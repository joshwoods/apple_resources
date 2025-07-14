

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  issuer 

Instance Property

# issuer

The issuer of the identity token that the identity provider returns.

macOS 13.0+

``` source
var issuer: String { get }
```

## Mentioned in 

Processing the JSON Web Encryption (JWE) login response

## See Also

### Obtaining the required configuration

var audience: String

The audience for validation and requests.

var clientID: String

The identifier for the client at the identity provider.

var jwksEndpointURL: URL

The JSON Web Key Set endpoint URL for keys.

var tokenEndpointURL: URL

The token endpoint URL for login requests.

