

- Foundation
- NSMutableURLRequest
-  httpBody 

Instance Property

# httpBody

The request body.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpBody: Data? { get set }
```

## Discussion

The request body is sent as the message body of the request, as in an HTTP `POST` request. Setting the HTTP body data clears any input stream in httpBodyStream. These values are mutually exclusive.

## See Also

### Accessing request components

var httpMethod: String

The HTTP request method.

var url: URL?

The URL being requested.

var httpBodyStream: InputStream?

The request body as an input stream.

var mainDocumentURL: URL?

The main document URL.

