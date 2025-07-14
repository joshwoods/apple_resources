

- Foundation
- DataProtocol
-  firstRange(of:) 

Instance Method

# firstRange(of:)

Returns the first found range of the type’s data buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func firstRange(of data: D) -> Range? where D : DataProtocol
```

## Parameters 

`data`  

The data sequence to find.

## Return Value

The range, if found, of the first match of the provided data sequence.

## Discussion

An example of searching a data buffer converted from a string:

```
let data = "0123456789".data(using: .utf8)!
let pattern = "456".data(using: .utf8)!
let foundRange = data.firstRange(of: pattern)

// foundRange == Range(4..

## See Also

### Searching Within Data

func firstRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the first found range of the type’s data buffer.

**Required** Default implementation provided.

func lastRange&lt;D>(of: D) -> Range&lt;Self.Index>?

Returns the last found range of the type’s data buffer.

func lastRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the last found range of the type’s data buffer.

**Required** Default implementation provided.

