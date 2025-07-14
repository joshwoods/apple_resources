

- Foundation
- NSURLRequest
-  mainDocumentURL 

Instance Property

# mainDocumentURL

The main document URL associated with the request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var mainDocumentURL: URL? { get }
```

## Discussion

This URL is used for the cookie “same domain as main document” policy.

## See Also

### Related Documentation

var mainDocumentURL: URL?

The main document URL.

### Accessing request components

var httpMethod: String?

The HTTP request method.

var url: URL?

The URL being requested.

var httpBody: Data?

The request body.

var httpBodyStream: InputStream?

The request body as an input stream.

