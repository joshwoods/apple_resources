

- Foundation
- NSCoder
-  error 

Instance Property

# error

An error in the top-level encode.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var error: (any Error)? { get }
```

## Discussion

The meaning of this property depends on the setting of the decodingFailurePolicy property. For NSCoder.DecodingFailurePolicy.raiseException, this property is always `nil`. For NSCoder.DecodingFailurePolicy.setErrorAndReturn, a non-`nil` value represents the first error encountered while decoding the archive.

## See Also

### Managing Decode Errors

func failWithError(any Error)

Signals to this coder that the decode operation has failed.

