

- Foundation
- HTTPCookie
-  requestHeaderFields(with:) 

Type Method

# requestHeaderFields(with:)

Converts an array of cookies to a dictionary of header fields.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func requestHeaderFields(with cookies: [HTTPCookie]) -> [String : String]
```

## Parameters 

`cookies`  

The cookies from which the header fields are created.

## Return Value

The dictionary of header fields created from the provided cookies.

## Discussion

To send these headers as part of a URL request to a remote server, create an NSMutableURLRequest object, then call the allHTTPHeaderFields or setValue(_:forHTTPHeaderField:) method to set the provided headers for the request. Finally, initialize and start an URLSessionTask instance based on that request object.

