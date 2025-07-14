

- ClassKit
- CLSErrorUserInfoKey
-  underlyingErrorsKey 

Type Property

# underlyingErrorsKey

A key whose value is the array of errors that contributed to this error.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
static let underlyingErrorsKey: CLSErrorUserInfoKey
```

## Discussion

This key only appears for errors with code partialFailure in Swift or CLSError.Code.partialFailure in Objective-C, signifying that more than one error occurred.

## See Also

### Keys

static let objectKey: CLSErrorUserInfoKey

A key whose value is the object that caused the error.

static let successfulObjectsKey: CLSErrorUserInfoKey

