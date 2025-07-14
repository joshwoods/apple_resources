

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  requestedOperation 

Instance Property

# requestedOperation

The operation for the extension to execute.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
var requestedOperation: ASAuthorizationProviderAuthorizationOperation { get }
```

## See Also

### Parsing the Request

var url: URL

The complete URL of the request, including all components.

var httpHeaders: [String : String]

The HTTP headers of the request.

var httpBody: Data

The HTTP body of the request.

var realm: String

The realm to which the request applies.

struct ASAuthorizationProviderAuthorizationOperation

A type that represents an authorization operation.

var authorizationOptions: [AnyHashable : Any]

A collection of options associated with the request.

