

- Foundation
- DataProtocol
-  firstRange(of:in:) 

Instance Method

# firstRange(of:in:)

Returns the first found range of the type’s data buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func firstRange(
    of: D,
    in: R
) -> Range? where D : DataProtocol, R : RangeExpression, Self.Index == R.Bound
```

**Required** Default implementation provided.

## Parameters 

`of`  

The data sequence to find.

`in`  

A range to limit the scope of the search.

## Return Value

The range, if found, of the first match of the provided data sequence.

## Discussion

An example of searching a constrained range within a data buffer for the first match:

```
let data: [UInt8] = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
let pattern: [UInt8] = [2, 3, 4]

let possibleMatch = data.firstRange(of: pattern, in: 5...9)
// possibleMatch == nil

let match = data.firstRange(of: pattern, in: 2...9)
// match == 2..

## Default Implementations

### DataProtocol Implementations

func firstRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the first found range of the type’s data buffer.

## See Also

### Searching Within Data

func firstRange&lt;D>(of: D) -> Range&lt;Self.Index>?

Returns the first found range of the type’s data buffer.

func lastRange&lt;D>(of: D) -> Range&lt;Self.Index>?

Returns the last found range of the type’s data buffer.

func lastRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the last found range of the type’s data buffer.

**Required** Default implementation provided.

