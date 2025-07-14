

- Foundation
- NSArray
-  sortedArray(\_:context:hint:) 

Instance Method

# sortedArray(\_:context:hint:)

Returns a new array that lists the receiving array’s elements in ascending order as defined by the comparison function `comparator`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sortedArray(
    _ comparator: (Any, Any, UnsafeMutableRawPointer?) -> Int,
    context: UnsafeMutableRawPointer?,
    hint: Data?
) -> [Any]
```

## Discussion

The new array contains references to the receiving array’s elements, not copies of them.

This method is similar to sortedArray(_:context:), except that it uses the supplied hint to speed the sorting process. When you know the array is nearly sorted, this method is faster than sortedArray(_:context:). If you sorted a large array (`N` entries) once, and you don’t change it much (`P` additions and deletions, where `P` is much smaller than `N`), then you can reuse the work you did in the original sort by conceptually doing a merge sort between the `N` “old” items and the `P` “new” items.

To obtain an appropriate hint, use sortedArrayHint. You should obtain this hint when the original array has been sorted, and keep hold of it until you need it, after the array has been modified. The hint is computed by sortedArrayHint in `O(N)` (where `N` is the number of items). This assumes that items in the array implement a `-hash` method. Given a suitable hint, and assuming that the hash function is a “good” hash function, -sortedArray(_:context:hint:) sorts the array in `O(P*LOG(P)+N)` where `P` is the number of adds or deletes. This is an improvement over the un-hinted sort, `O(N*LOG(N))`, when `P` is small.

The hint is simply an array of size `N` containing the `N` hashes. To re-sort you need internally to create a map table mapping a hash to the index. Using this map table on the new array, you can get a first guess for the indexes, and then sort that. For example, a sorted array {A, B, D, E, F} with corresponding hash values {25, 96, 78, 32, 17}, may be subject to small changes that result in contents {E, A, C, B, F}. The mapping table maps the hashes {25, 96, 78, 32, 17} to the indexes {#0, \#1, \#2, \#3, \#4}. If the hashes for {E, A, C, B, F} are {32, 25, 99, 96, 17}, then by using the mapping table you can get a first order sort {#3, \#0, ?, \#1, \#4}, so therefore create an initial semi-sorted array {A, B, E, F}, and then perform a cheap merge sort with {C} that yields {A, B, C, E, F}.

## See Also

### Sorting

var sortedArrayHint: Data

Analyzes the array and returns a “hint” that speeds the sorting of the array when the hint is supplied to sortedArray(_:context:hint:).

func sortedArray((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?) -> [Any]

Returns a new array that lists the receiving array’s elements in ascending order as defined by the comparison function `comparator`.

func sortedArray(using: [NSSortDescriptor]) -> [Any]

Returns a copy of the receiving array sorted as specified by a given array of sort descriptors.

func sortedArray(using: Selector) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given selector.

func sortedArray(comparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

func sortedArray(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

typealias Comparator

Defines the signature for a block object used for comparison operations.

