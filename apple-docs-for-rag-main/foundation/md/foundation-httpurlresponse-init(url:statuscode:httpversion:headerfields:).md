

- Foundation
- HTTPURLResponse
-  init(url:statusCode:httpVersion:headerFields:) 

Initializer

# init(url:statusCode:httpVersion:headerFields:)

Initializes an HTTP URL response object with a status code, protocol version, and response headers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    url: URL,
    statusCode: Int,
    httpVersion HTTPVersion: String?,
    headerFields: [String : String]?
)
```

## Parameters 

`url`  

The URL from which the response was generated.

`statusCode`  

The HTTP status code to return (`404`, for example). See RFC 2616 for details.

`HTTPVersion`  

The version of the HTTP response as returned by the server. This is typically represented as “HTTP/1.1”.

`headerFields`  

A dictionary representing the keys and values from the server’s response header.

## Return Value

An initialized HTTPURLResponse object or `nil` if an error occurred during initialization.

