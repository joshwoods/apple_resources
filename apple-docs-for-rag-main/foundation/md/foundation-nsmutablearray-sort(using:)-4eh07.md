

- Foundation
- NSMutableArray
-  sort(using:) 

Instance Method

# sort(using:)

Sorts the receiver using a given array of sort descriptors.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sort(using sortDescriptors: [NSSortDescriptor])
```

## Parameters 

`sortDescriptors`  

An array containing the `NSSortDescriptor` objects to use to sort the receiving array’s contents.

## Discussion

See NSSortDescriptor for additional information.

## See Also

### Related Documentation

func sortedArray(using: [NSSortDescriptor]) -> [Any]

Returns a copy of the receiving array sorted as specified by a given array of sort descriptors.

### Rearranging Content

func exchangeObject(at: Int, withObjectAt: Int)

Exchanges the objects in the array at given indexes.

func sort(comparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the comparison method specified by a given Comparator block.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the specified options and the comparison method specified by a given Comparator block.

func sort((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?)

Sorts the receiver in ascending order as defined by the comparison function `compare`.

func sort(using: Selector)

Sorts the receiver in ascending order, as determined by the comparison method specified by a given selector.

