

- Foundation
- NSMutableArray
-  exchangeObject(at:withObjectAt:) 

Instance Method

# exchangeObject(at:withObjectAt:)

Exchanges the objects in the array at given indexes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func exchangeObject(
    at idx1: Int,
    withObjectAt idx2: Int
)
```

## Parameters 

`idx1`  

The index of the object with which to replace the object at index `idx2`.

`idx2`  

The index of the object with which to replace the object at index `idx1`.

## See Also

### Rearranging Content

func sort(using: [NSSortDescriptor])

Sorts the receiver using a given array of sort descriptors.

func sort(comparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the comparison method specified by a given Comparator block.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the specified options and the comparison method specified by a given Comparator block.

func sort((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?)

Sorts the receiver in ascending order as defined by the comparison function `compare`.

func sort(using: Selector)

Sorts the receiver in ascending order, as determined by the comparison method specified by a given selector.

