

- Swift
- SingleValueEncodingContainer
-  encodeNil() 

Instance Method

# encodeNil()

Encodes a null value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encodeNil() throws
```

**Required**

## Discussion

Throws

`EncodingError.invalidValue` if a null value is invalid in the current context for this format.

Precondition

May not be called after a previous `self.encode(_:)` call.

