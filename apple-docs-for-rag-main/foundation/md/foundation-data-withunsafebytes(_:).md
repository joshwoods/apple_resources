

- Foundation
- Data
-  withUnsafeBytes(\_:) 

Instance Method

# withUnsafeBytes(\_:)

Accesses the raw bytes in the data’s buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
func withUnsafeBytes(_ body: (UnsafePointer) throws -> ResultType) rethrows -> ResultType
```

## Discussion

Warning

The byte pointer argument should not be stored and used outside of the lifetime of the call to the closure.

## See Also

### Accessing Underlying Memory

func withUnsafeMutableBytes&lt;ResultType, ContentType>((UnsafeMutablePointer&lt;ContentType>) throws -> ResultType) rethrows -> ResultType

Mutates the raw bytes in the data’s buffer.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, count: Int)

Copies the contents of the data to memory.

func copyBytes(to: UnsafeMutablePointer&lt;UInt8>, from: Range&lt;Data.Index>)

Copies a subset of the contents of the data to memory.

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>, from: Range&lt;Data.Index>?) -> Int

Copies the bytes in a range from the data into a buffer.

