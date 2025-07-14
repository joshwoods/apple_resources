

- Foundation
- NSMutableURLRequest
-  httpBodyStream 

Instance Property

# httpBodyStream

The request body as an input stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpBodyStream: InputStream? { get set }
```

## Discussion

The request body of the receiver will be this input stream. The entire contents of the stream will be sent as the body, as in an HTTP `POST` request. The input stream should be unopened and the receiver will take over as the stream’s delegate.

Setting a body stream clears any data in httpBody. These values are mutually exclusive.

## See Also

### Accessing request components

var httpMethod: String

The HTTP request method.

var url: URL?

The URL being requested.

var httpBody: Data?

The request body.

var mainDocumentURL: URL?

The main document URL.

