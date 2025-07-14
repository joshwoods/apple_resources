

- Foundation
- MutableDataProtocol
-  resetBytes(in:) 

Instance Method

# resetBytes(in:)

Replaces the contents of the data buffer with zeros for the provided range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func resetBytes(in range: R) where R : RangeExpression, Self.Index == R.Bound
```

**Required** Default implementation provided.

## Parameters 

`range`  

The range of bytes to replace with zeros.

## Discussion

The following example sets the bytes to zero for the bytes identified by the provided range:

```
var dest: [UInt8] = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
dest.resetBytes(in: 1...3)
// dest = [0xFF, 0x00, 0x00, 0x00, 0xFF, 0xFF]
```

## Default Implementations

### MutableDataProtocol Implementations

func resetBytes&lt;R>(in: R)

Replaces the contents of the data buffer with zeros for the provided range.

