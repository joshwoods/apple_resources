

- Foundation
- NSArray
-  sortedArray(comparator:) 

Instance Method

# sortedArray(comparator:)

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sortedArray(comparator cmptr: (Any, Any) -> ComparisonResult) -> [Any]
```

## Parameters 

`cmptr`  

A comparator block.

## Return Value

An array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified `cmptr`.

## See Also

### Sorting

var sortedArrayHint: Data

Analyzes the array and returns a “hint” that speeds the sorting of the array when the hint is supplied to sortedArray(_:context:hint:).

func sortedArray((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?) -> [Any]

Returns a new array that lists the receiving array’s elements in ascending order as defined by the comparison function `comparator`.

func sortedArray((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?, hint: Data?) -> [Any]

Returns a new array that lists the receiving array’s elements in ascending order as defined by the comparison function `comparator`.

func sortedArray(using: [NSSortDescriptor]) -> [Any]

Returns a copy of the receiving array sorted as specified by a given array of sort descriptors.

func sortedArray(using: Selector) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given selector.

func sortedArray(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

typealias Comparator

Defines the signature for a block object used for comparison operations.

