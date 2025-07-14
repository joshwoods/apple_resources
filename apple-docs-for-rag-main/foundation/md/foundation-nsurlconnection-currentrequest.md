

- Foundation
- NSURLConnection
-  currentRequest 

Instance Property

# currentRequest

The current connection request.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var currentRequest: URLRequest { get }
```

## Discussion

As the connection performs the load, the request may change as a result of protocol canonicalization or due to following redirects. This property provides the current value of the request.

## See Also

### Connection URL Information

var originalRequest: URLRequest

A deep copy of the original connection request.

