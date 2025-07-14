

- Foundation
- NSMutableArray
-  sort(using:) 

Instance Method

# sort(using:)

Sorts the receiver in ascending order, as determined by the comparison method specified by a given selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sort(using comparator: Selector)
```

## Parameters 

`comparator`  

A selector that specifies the comparison method to use to compare elements in the array.

The `comparator` message is sent to each object in the array and has as its single argument another object in the array. The `comparator` method should return `NSOrderedAscending` if the array is smaller than the argument, `NSOrderedDescending` if the array is larger than the argument, and `NSOrderedSame` if they are equal.

## See Also

### Related Documentation

func sortedArray(using: Selector) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given selector.

### Rearranging Content

func exchangeObject(at: Int, withObjectAt: Int)

Exchanges the objects in the array at given indexes.

func sort(using: [NSSortDescriptor])

Sorts the receiver using a given array of sort descriptors.

func sort(comparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the comparison method specified by a given Comparator block.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the specified options and the comparison method specified by a given Comparator block.

func sort((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?)

Sorts the receiver in ascending order as defined by the comparison function `compare`.

