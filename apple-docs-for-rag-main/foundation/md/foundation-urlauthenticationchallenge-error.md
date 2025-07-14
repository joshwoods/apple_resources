

- Foundation
- URLAuthenticationChallenge
-  error 

Instance Property

# error

The error object representing the last authentication failure.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var error: (any Error)? { get }
```

## Discussion

This value is `nil` if the protocol doesn’t use errors to indicate an authentication failure.

## See Also

### Related Documentation

var failureResponse: URLResponse?

The URL response object representing the last authentication failure.

