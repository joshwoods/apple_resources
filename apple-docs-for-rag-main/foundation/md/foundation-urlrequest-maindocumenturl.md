

- Foundation
- URLRequest
-  mainDocumentURL 

Instance Property

# mainDocumentURL

The main document URL associated with this request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var mainDocumentURL: URL? { get set }
```

## Discussion

This URL is used for the cookie “same domain as main document” policy.

## See Also

### Accessing request components

var httpMethod: String?

The HTTP request method.

var url: URL?

The URL of the request.

var httpBody: Data?

The data sent as the message body of a request, such as for an HTTP POST request.

var httpBodyStream: InputStream?

The stream used to deliver the HTTP body.

