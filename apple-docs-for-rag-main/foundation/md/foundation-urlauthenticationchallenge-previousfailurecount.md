

- Foundation
- URLAuthenticationChallenge
-  previousFailureCount 

Instance Property

# previousFailureCount

The receiver’s count of failed authentication attempts.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var previousFailureCount: Int { get }
```

## Discussion

The previous failure count includes failures from *all* protection spaces, not just the current one.

## See Also

### Getting properties of previous authentication attempts

var failureResponse: URLResponse?

The URL response object representing the last authentication failure.

var proposedCredential: URLCredential?

The proposed credential for this challenge.

