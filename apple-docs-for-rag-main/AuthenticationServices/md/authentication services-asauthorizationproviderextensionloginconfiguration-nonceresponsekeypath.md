

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  nonceResponseKeypath 

Instance Property

# nonceResponseKeypath

The keypath in the response that contains the one-time use value.

macOS 13.0+

``` source
var nonceResponseKeypath: String { get set }
```

## Mentioned in 

Obtaining a server nonce

## Discussion

## See Also

### Configuring the server nonce

var customNonceRequestValues: [URLQueryItem]

Custom values to add to the server nonce POST request body.

var nonceEndpointURL: URL

The URL to retrieve a one-time use value from the server.

var serverNonceClaimName: String

The name of the claim to include in authentication requests.

