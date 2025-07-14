

- Foundation
- NSUserActivity
- NSUserActivity.TypedPayloadError
-  NSUserActivity.TypedPayloadError.encodingError 

Case

# NSUserActivity.TypedPayloadError.encodingError

An encoding error that indicates that the content failed to encode into a valid dictionary.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case encodingError
```

## Discussion

The setTypedPayload(_:) method throws this error.

## See Also

### Typed payload errors

case invalidContent

A decoding error that indicates that the user info dictionary is empty or invalid.

