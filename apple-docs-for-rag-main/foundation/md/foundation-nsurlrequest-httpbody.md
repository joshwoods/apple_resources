

- Foundation
- NSURLRequest
-  httpBody 

Instance Property

# httpBody

The request body.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpBody: Data? { get }
```

## Discussion

This data is sent as the message body of a request, as in an HTTP `POST` request.

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

var httpBodyStream: InputStream?

The request body as an input stream.

var mainDocumentURL: URL?

The main document URL associated with the request.

