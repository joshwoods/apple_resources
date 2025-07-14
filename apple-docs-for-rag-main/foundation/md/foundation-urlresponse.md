

- Foundation
-  URLResponse 

Class

# URLResponse

The metadata associated with the response to a URL load request, independent of protocol and URL scheme.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLResponse
```

## Mentioned in 

Processing URL session data task results with Combine

Downloading files from websites

## Overview

The related HTTPURLResponse class is a commonly used subclass of URLResponse whose objects represent a response to an HTTP URL load request and store additional protocol-specific information such as the response headers. Whenever you make an HTTP request, the URLResponse object you get back is actually an instance of the HTTPURLResponse class.

Note

URLResponse objects don’t contain the actual bytes representing the content of a URL. Instead, the data is returned either a piece at a time through delegate calls or in its entirety when the request completes, depending on the method and class used to initiate the request.

Read Fetching website data into memory to learn various ways to receive the content data from a URL load.

## Topics

### Creating a response

init(url: URL, mimeType: String?, expectedContentLength: Int, textEncodingName: String?)

Creates an initialized URLResponse object with the URL, MIME type, length, and text encoding set to given values.

### Getting the response properties

var expectedContentLength: Int64

The expected length of the response’s content.

var suggestedFilename: String?

A suggested filename for the response data.

var mimeType: String?

The MIME type of the response.

var textEncodingName: String?

The name of the text encoding provided by the response’s originating source.

var url: URL?

The URL for the response.

## Relationships

### Inherits From

- NSObject

### Inherited By

- HTTPURLResponse

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Requests and responses

struct URLRequest

A URL load request that is independent of protocol or URL scheme.

class NSURLRequest

A URL load request that is independent of protocol or URL scheme.

class NSMutableURLRequest

A mutable URL load request that is independent of protocol or URL scheme.

class HTTPURLResponse

The metadata associated with the response to an HTTP protocol URL load request.

