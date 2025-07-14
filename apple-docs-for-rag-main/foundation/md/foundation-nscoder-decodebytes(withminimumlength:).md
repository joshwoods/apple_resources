

- Foundation
- NSCoder
-  decodeBytes(withMinimumLength:) 

Instance Method

# decodeBytes(withMinimumLength:)

Decode bytes from the decoder. The length of the bytes must be greater than or equal to the `length` parameter. If the result exists, but is of insufficient length, then the decoder uses `failWithError` to fail the entire decode operation. The result of that is configurable on a per-NSCoder basis using `NSDecodingFailurePolicy`.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func decodeBytes(withMinimumLength length: Int) -> UnsafeMutableRawPointer?
```

