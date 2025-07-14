

- RealityKit
- QueryResult
-  dropLast(\_:) 

Instance Method

# dropLast(\_:)

Returns a sequence containing all but the given number of final elements.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func dropLast(_ k: Int = 1) -> [Self.Element]
```

## Parameters 

`n`  

The number of elements to drop off the end of the sequence. `n` must be greater than or equal to zero.

## Return Value

A sequence leaving off the specified number of elements.

## Discussion

The sequence must be finite. If the number of elements to drop exceeds the number of elements in the sequence, the result is an empty sequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.dropLast(2))
// Prints "[1, 2, 3]"
print(numbers.dropLast(10))
// Prints "[]"
```

Complexity

O(*n*), where *n* is the length of the sequence.

