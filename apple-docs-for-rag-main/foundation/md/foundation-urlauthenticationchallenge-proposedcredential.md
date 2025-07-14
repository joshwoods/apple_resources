

- Foundation
- URLAuthenticationChallenge
-  proposedCredential 

Instance Property

# proposedCredential

The proposed credential for this challenge.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var proposedCredential: URLCredential? { get }
```

## Discussion

This method returns `nil` if there is no default credential for this challenge.

If you have previously attempted to authenticate and failed, this method returns the most recent failed credential.

If the proposed credential is not `nil` and returns true when you call its hasPassword method, then the credential is ready to use as-is. If the proposed credential’s hasPassword method returns false, then the credential provides a default user name, and the client must prompt the user for a corresponding password.

## See Also

### Getting properties of previous authentication attempts

var failureResponse: URLResponse?

The URL response object representing the last authentication failure.

var previousFailureCount: Int

The receiver’s count of failed authentication attempts.

