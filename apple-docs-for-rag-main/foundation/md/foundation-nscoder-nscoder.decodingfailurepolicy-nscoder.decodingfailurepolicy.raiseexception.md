

- Foundation
- NSCoder
- NSCoder.DecodingFailurePolicy
-  NSCoder.DecodingFailurePolicy.raiseException 

Case

# NSCoder.DecodingFailurePolicy.raiseException

A failure policy that directs the coder to raise an exception.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case raiseException
```

## Discussion

With this policy, the NSCoder raises an exception internally to propagate failure messages (and unwind the stack). In Objective-C, this exception can be transformed into an NSError via methods like decodeTopLevelObjectAndReturnError:

## See Also

### Failure Policies

case setErrorAndReturn

A failure policy that directs the coder to capture the failure as an error object.

case setErrorAndReturn

A failure policy that directs the coder to capture the failure as an error object.

