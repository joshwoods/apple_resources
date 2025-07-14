

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  customNonceRequestValues 

Instance Property

# customNonceRequestValues

Custom values to add to the server nonce POST request body.

macOS 13.0+

``` source
var customNonceRequestValues: [URLQueryItem] { get set }
```

## Mentioned in 

Obtaining a server nonce

## See Also

### Configuring the server nonce

var nonceEndpointURL: URL

The URL to retrieve a one-time use value from the server.

var nonceResponseKeypath: String

The keypath in the response that contains the one-time use value.

var serverNonceClaimName: String

The name of the claim to include in authentication requests.

