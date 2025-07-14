

- Foundation
- NSMutableURLRequest
-  mainDocumentURL 

Instance Property

# mainDocumentURL

The main document URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var mainDocumentURL: URL? { get set }
```

## Discussion

The caller should set the main document URL to an appropriate main document, if known. For example, when loading a web page the URL of the HTML document for the top-level frame would be appropriate. This URL will be used for the “only from same domain as main document” cookie accept policy.

`nil` indicates no main document.

## See Also

### Accessing request components

var httpMethod: String

The HTTP request method.

var url: URL?

The URL being requested.

var httpBody: Data?

The request body.

var httpBodyStream: InputStream?

The request body as an input stream.

