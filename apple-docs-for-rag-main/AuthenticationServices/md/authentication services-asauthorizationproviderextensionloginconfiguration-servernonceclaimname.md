

- Authentication Services
- ASAuthorizationProviderExtensionLoginConfiguration
-  serverNonceClaimName 

Instance Property

# serverNonceClaimName

The name of the claim to include in authentication requests.

macOS 13.0+

``` source
var serverNonceClaimName: String { get set }
```

## Mentioned in 

Supporting key requests and key exchange requests

Creating an embedded assertion

Creating a refresh request

Creating an encrypted embedded assertion

Creating and validating a login request

## Discussion

The default value is `request_nonce`.

## See Also

### Configuring the server nonce

var customNonceRequestValues: [URLQueryItem]

Custom values to add to the server nonce POST request body.

var nonceEndpointURL: URL

The URL to retrieve a one-time use value from the server.

var nonceResponseKeypath: String

The keypath in the response that contains the one-time use value.

