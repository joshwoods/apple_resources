

- Foundation
-  HTTPURLResponse 

Class

# HTTPURLResponse

The metadata associated with the response to an HTTP protocol URL load request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class HTTPURLResponse
```

## Overview

The HTTPURLResponse class is a subclass of URLResponse that provides methods for accessing information specific to HTTP protocol responses. Whenever you make HTTP URL load requests, any response objects you get back from the URLSession, NSURLConnection, or NSURLDownload class are instances of the HTTPURLResponse class.

## Topics

### Initializing a response object

init?(url: URL, statusCode: Int, httpVersion: String?, headerFields: [String : String]?)

Initializes an HTTP URL response object with a status code, protocol version, and response headers.

### Getting HTTP response headers

var allHeaderFields: [AnyHashable : Any]

All HTTP header fields of the response.

func value(forHTTPHeaderField: String) -> String?

Returns the value that corresponds to the given header field.

### Getting response status codes

class func localizedString(forStatusCode: Int) -> String

Returns a localized string corresponding to a specified HTTP status code.

var statusCode: Int

The response’s HTTP status code.

## Relationships

### Inherits From

- URLResponse

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

class URLResponse

The metadata associated with the response to a URL load request, independent of protocol and URL scheme.

