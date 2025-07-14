

- Foundation
- NSURLRequest
-  httpBodyStream 

Instance Property

# httpBodyStream

The request body as an input stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpBodyStream: InputStream? { get }
```

## Discussion

`nil` if the body stream has not been set. The returned stream is for examination only—it is not safe to manipulate the stream in any way.

The receiver will have either an HTTP body or an HTTP body stream, only one may be set for a request. A HTTP body stream is preserved when copying an NSURLRequest object, but is lost when a request is archived using the NSCoding protocol.

## See Also

### Related Documentation

var httpBodyStream: InputStream?

The request body as an input stream.

var httpBody: Data?

The request body.

### Accessing request components

var httpMethod: String?

The HTTP request method.

var url: URL?

The URL being requested.

var httpBody: Data?

The request body.

var mainDocumentURL: URL?

The main document URL associated with the request.

