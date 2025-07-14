

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  jwksEndpointURL 

Instance Property

# jwksEndpointURL

The JSON Web Key Set endpoint URL for keys.

macOS 13.0+

``` source
var jwksEndpointURL: URL { get set }
```

## Mentioned in 

Processing the JSON Web Encryption (JWE) login response

## See Also

### Obtaining the required configuration

var audience: String

The audience for validation and requests.

var clientID: String

The identifier for the client at the identity provider.

var tokenEndpointURL: URL

The token endpoint URL for login requests.

var issuer: String

The issuer of the identity token that the identity provider returns.

