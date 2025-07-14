

- Foundation
- NSMutableURLRequest
-  httpMethod 

Instance Property

# httpMethod

The HTTP request method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpMethod: String { get set }
```

## Discussion

The default HTTP method is “GET”.

## See Also

### Accessing request components

var url: URL?

The URL being requested.

var httpBody: Data?

The request body.

var httpBodyStream: InputStream?

The request body as an input stream.

var mainDocumentURL: URL?

The main document URL.

