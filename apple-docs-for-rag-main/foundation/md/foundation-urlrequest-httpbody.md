

- Foundation
- URLRequest
-  httpBody 

Instance Property

# httpBody

The data sent as the message body of a request, such as for an HTTP POST request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpBody: Data? { get set }
```

## See Also

### Accessing request components

var httpMethod: String?

The HTTP request method.

var url: URL?

The URL of the request.

var httpBodyStream: InputStream?

The stream used to deliver the HTTP body.

var mainDocumentURL: URL?

The main document URL associated with this request.

