

- Foundation
- Data
-  enumerateBytes(\_:) 

Instance Method

# enumerateBytes(\_:)

Enumerates the contents of the data’s buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
func enumerateBytes(_ block: (UnsafeBufferPointer, Data.Index, inout Bool) -> Void)
```

## Parameters 

`block`  

The closure to invoke for each region of data. You may stop the enumeration by setting the `stop` parameter to `true`.

## Discussion

In some cases, (for example, a Data backed by a `dispatch_data_t`, the bytes may be stored discontiguously. In those cases, this function invokes the closure for each contiguous region of bytes.

## See Also

### Iterating Over Bytes

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func makeIterator() -> Data.Iterator

Returns an iterator over the contents of the data.

