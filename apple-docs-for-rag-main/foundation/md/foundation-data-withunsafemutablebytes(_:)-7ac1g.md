

- Foundation
- Data
-  withUnsafeMutableBytes(\_:) 

Instance Method

# withUnsafeMutableBytes(\_:)

Mutates the raw bytes in the data’s buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
mutating func withUnsafeMutableBytes(_ body: (UnsafeMutablePointer) throws -> ResultType) rethrows -> ResultType
```

## Discussion

This function assumes that you are mutating the contents.

Warning

The byte pointer argument should not be stored and used outside of the lifetime of the call to the closure.

## See Also

### Accessing Underlying Memory

func withUnsafeBytes&lt;ResultType, ContentType>((UnsafePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Accesses the raw bytes in the data’s buffer.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

Copies the contents of the data to memory.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;Data.Index>)

Copies a subset of the contents of the data to memory.

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: Range&lt;Data.Index>?) -> Int

Copies the bytes in a range from the data into a buffer.

