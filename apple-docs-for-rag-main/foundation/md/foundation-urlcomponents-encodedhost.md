

- Foundation
- URLComponents
-  encodedHost 

Instance Property

# encodedHost

The host subcomponent, percent-encoded.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var encodedHost: String? { get set }
```

## Discussion

The getter for this property retains any percent-encoding this component may have. Setting this property assumes the component string already has the correct percent-encoding. Attempting to set an incorrectly percent-encoded string raises fatalError(_:file:line:).

## See Also

### Accessing components in native format

var fragment: String?

The fragment subcomponent.

var host: String?

The host subcomponent.

var password: String?

The password subcomponent of the URL.

var path: String

The path subcomponent.

var port: Int?

The port subcomponent.

var query: String?

The query subcomponent.

var queryItems: [URLQueryItem]?

An array of query items for the URL in the order in which they appear in the original query string.

var scheme: String?

The scheme subcomponent of the URL.

var user: String?

The user subcomponent of the URL.

