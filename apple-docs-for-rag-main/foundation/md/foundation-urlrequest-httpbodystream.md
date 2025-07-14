

- Foundation
- URLRequest
-  httpBodyStream 

Instance Property

# httpBodyStream

The stream used to deliver the HTTP body.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpBodyStream: InputStream? { get set }
```

## Discussion

The stream is returned for examination only; it’s unsafe for the caller to manipulate the stream in any way.

Note

The httpBodyStream and httpBody are mutually exclusive - only one can be set on a given request. The body stream is preserved across copies, but is lost when the request is coded via the NSCoding protocol

## See Also

### Accessing request components

var httpMethod: String?

The HTTP request method.

var url: URL?

The URL of the request.

var httpBody: Data?

The data sent as the message body of a request, such as for an HTTP POST request.

var mainDocumentURL: URL?

The main document URL associated with this request.

