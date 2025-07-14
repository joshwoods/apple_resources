

- Foundation
- URLResponse
-  textEncodingName 

Instance Property

# textEncodingName

The name of the text encoding provided by the response’s originating source.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var textEncodingName: String? { get }
```

## Discussion

If no text encoding was provided by the protocol, this property’s value is `nil`.

You can convert this string to a `CFStringEncoding` value by calling CFStringConvertIANACharSetNameToEncoding(_:). You can subsequently convert that value to an `NSStringEncoding` value by calling CFStringConvertEncodingToNSStringEncoding(_:).

## See Also

### Getting the response properties

var expectedContentLength: Int64

The expected length of the response’s content.

var suggestedFilename: String?

A suggested filename for the response data.

var mimeType: String?

The MIME type of the response.

var url: URL?

The URL for the response.

