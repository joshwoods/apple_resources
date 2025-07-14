

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  nonceEndpointURL 

Instance Property

# nonceEndpointURL

The URL to retrieve a one-time use value from the server.

macOS 13.0+

``` source
var nonceEndpointURL: URL { get set }
```

## Mentioned in 

Obtaining a server nonce

## Discussion

The value of this property defaults to tokenEndpointURL.

## See Also

### Configuring the server nonce

var customNonceRequestValues: [URLQueryItem]

Custom values to add to the server nonce POST request body.

var nonceResponseKeypath: String

The keypath in the response that contains the one-time use value.

var serverNonceClaimName: String

The name of the claim to include in authentication requests.

