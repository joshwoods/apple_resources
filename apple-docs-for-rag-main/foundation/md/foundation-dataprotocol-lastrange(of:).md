

- Foundation
- DataProtocol
-  lastRange(of:) 

Instance Method

# lastRange(of:)

Returns the last found range of the type’s data buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lastRange(of data: D) -> Range? where D : DataProtocol
```

## Parameters 

`data`  

The data sequence to find.

## Return Value

The range, if found, of the last match of the provided data sequence.

## Discussion

An example of searching a data buffer for the last match:

```
let data: [UInt8] = [0, 1, 2, 3, 0, 1, 2, 3]
let pattern: [UInt8] = [2, 3]

let match = data.lastRange(of: pattern)
// match == 6..

## See Also

### Searching Within Data

func firstRange&lt;D>(of: D) -> Range&lt;Self.Index>?

Returns the first found range of the type’s data buffer.

func firstRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the first found range of the type’s data buffer.

**Required** Default implementation provided.

func lastRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the last found range of the type’s data buffer.

**Required** Default implementation provided.

