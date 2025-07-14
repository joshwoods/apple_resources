

- Security
- SecTrustResultType
-  SecTrustResultType.otherError 

Case

# SecTrustResultType.otherError

A value that indicates a failure other than trust evaluation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case otherError
```

## Discussion

This value indicates that evaluation failed for some other reason. This can be caused by either a revoked certificate or by OS-level errors that are unrelated to the certificates themselves.

You might receive the SecTrustResultType.otherError value after an evaluation, but you can’t store the value as part of the user trust settings with a call to the SecTrustSettingsSetTrustSettings(_:_:_:) method.

