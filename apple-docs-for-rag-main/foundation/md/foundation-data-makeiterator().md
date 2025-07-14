

- Foundation
- Data
-  makeIterator() 

Instance Method

# makeIterator()

Returns an iterator over the contents of the data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func makeIterator() -> Data.Iterator
```

## Discussion

The iterator will increment byte-by-byte.

## See Also

### Iterating Over Bytes

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func enumerateBytes((UnsafeBufferPointer&lt;UInt8>, Data.Index, inout Bool) -> Void)

Enumerates the contents of the data’s buffer.

