

- Foundation
- URLResponse
-  init(url:mimeType:expectedContentLength:textEncodingName:) 

Initializer

# init(url:mimeType:expectedContentLength:textEncodingName:)

Creates an initialized URLResponse object with the URL, MIME type, length, and text encoding set to given values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    url URL: URL,
    mimeType MIMEType: String?,
    expectedContentLength length: Int,
    textEncodingName name: String?
)
```

## Parameters 

`URL`  

The URL for the new object.

`MIMEType`  

The MIME type.

`length`  

The expected content length.This value should be `–1` if the expected length is undetermined

`name`  

The text encoding name. This value may be `nil`.

## Return Value

The initialized URL response.

## Discussion

This is the designated initializer for URLResponse.

## See Also

### Related Documentation

init?(url: URL, statusCode: Int, httpVersion: String?, headerFields: [String : String]?)

Initializes an HTTP URL response object with a status code, protocol version, and response headers.

