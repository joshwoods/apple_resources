

- Foundation
- NSURLConnection
-  originalRequest 

Instance Property

# originalRequest

A deep copy of the original connection request.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var originalRequest: URLRequest { get }
```

## Discussion

As the connection performs the load, the request may change as a result of protocol canonicalization or due to following redirects. currentRequest can be used to retrieve this value.

## See Also

### Connection URL Information

var currentRequest: URLRequest

The current connection request.

