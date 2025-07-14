

- Foundation
- URLAuthenticationChallenge
-  failureResponse 

Instance Property

# failureResponse

The URL response object representing the last authentication failure.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var failureResponse: URLResponse? { get }
```

## Discussion

This value is `nil` if the protocol doesn’t use responses to indicate an authentication failure.

## See Also

### Related Documentation

var error: (any Error)?

The error object representing the last authentication failure.

### Getting properties of previous authentication attempts

var previousFailureCount: Int

The receiver’s count of failed authentication attempts.

var proposedCredential: URLCredential?

The proposed credential for this challenge.

