

- Foundation
- URLComponents
-  port 

Instance Property

# port

The port subcomponent.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var port: Int? { get set }
```

## Discussion

The getter for this property removes any percent encoding this component may have (if the component allows percent encoding). Setting this property assumes the subcomponent or component string is not percent encoded and will add percent encoding (if the component allows percent encoding). Attempting to set a negative port number will cause a fatal error.

## See Also

### Accessing components in native format

var fragment: String?

The fragment subcomponent.

var host: String?

The host subcomponent.

var encodedHost: String?

The host subcomponent, percent-encoded.

var password: String?

The password subcomponent of the URL.

var path: String

The path subcomponent.

var query: String?

The query subcomponent.

var queryItems: [URLQueryItem]?

An array of query items for the URL in the order in which they appear in the original query string.

var scheme: String?

The scheme subcomponent of the URL.

var user: String?

The user subcomponent of the URL.

