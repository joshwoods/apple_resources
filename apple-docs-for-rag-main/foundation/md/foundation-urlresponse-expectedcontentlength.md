

- Foundation
- URLResponse
-  expectedContentLength 

Instance Property

# expectedContentLength

The expected length of the response’s content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var expectedContentLength: Int64 { get }
```

## Discussion

This property’s value is NSURLResponseUnknownLength if the length can’t be determined.

Some protocol implementations report the content length as part of the response, but not all protocols guarantee to deliver that amount of data. Your app should be prepared to deal with more or less data.

## See Also

### Getting the response properties

var suggestedFilename: String?

A suggested filename for the response data.

var mimeType: String?

The MIME type of the response.

var textEncodingName: String?

The name of the text encoding provided by the response’s originating source.

var url: URL?

The URL for the response.

