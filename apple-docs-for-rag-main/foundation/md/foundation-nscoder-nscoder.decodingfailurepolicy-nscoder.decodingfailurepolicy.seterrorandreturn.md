

- Foundation
- NSCoder
- NSCoder.DecodingFailurePolicy
-  NSCoder.DecodingFailurePolicy.setErrorAndReturn 

Case

# NSCoder.DecodingFailurePolicy.setErrorAndReturn

A failure policy that directs the coder to capture the failure as an error object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case setErrorAndReturn
```

## Discussion

On decode failure, the NSCoder will capture the failure as an NSError, and prevent further decodes (by returning `0` / `nil` equivalent as appropriate).

Use this policy if you know that all encoded objects use failWithError(_:) to communicate decode failures and don’t raise exceptions for error propagation.

## See Also

### Failure Policies

case raiseException

A failure policy that directs the coder to raise an exception.

case raiseException

A failure policy that directs the coder to raise an exception.

