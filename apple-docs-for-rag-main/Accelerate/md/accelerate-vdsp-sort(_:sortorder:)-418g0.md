

- Accelerate
- vDSP
-  sort(\_:sortOrder:) 

Type Method

# sort(\_:sortOrder:)

Sorts a vector of double-precision values in-place.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func sort(
    _ vector: inout V,
    sortOrder: vDSP.SortOrder
) where V : AccelerateMutableBuffer, V.Element == Double
```

## Parameters 

`vector`  

The array to sort.

`sortOrder`  

The sort order.

## Discussion

The single- and double-precision sort(_:sortOrder:) functions sort an array in place.

The following code sorts an array in ascending order, followed by decending order:

```
var values: [Float] = [4.0, 8.0, 3.0, 0.0, 7.0, 5.0, 9.0, 2.0, 6.0, 1.0]

vDSP.sort(&values,
          sortOrder: .ascending)

// Prints "[0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0]".
print(values)

vDSP.sort(&values,
          sortOrder: .descending)

// Prints "[9.0, 8.0, 7.0, 6.0, 5.0, 4.0, 3.0, 2.0, 1.0, 0.0]".
print(values)
```

## See Also

### Vector sorting functions

static func sort&lt;V>(inout V, sortOrder: vDSP.SortOrder)

Sorts a vector of single-precision values in-place.

enum SortOrder

Constants that specify the sorting order.

