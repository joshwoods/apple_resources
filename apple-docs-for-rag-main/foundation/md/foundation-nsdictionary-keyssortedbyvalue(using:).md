

- Foundation
- NSDictionary
-  keysSortedByValue(using:) 

Instance Method

# keysSortedByValue(using:)

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func keysSortedByValue(using comparator: Selector) -> [Any]
```

## Parameters 

`comparator`  

A selector that specifies the method to use to compare the values in the dictionary.

The `comparator` method should return `NSOrderedAscending` if the dictionary value is smaller than the argument, `NSOrderedDescending` if the dictionary value is larger than the argument, and `NSOrderedSame` if they are equal.

## Return Value

An array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values.

## Discussion

Pairs of dictionary values are compared using the comparison method specified by `comparator`; the `comparator` message is sent to one of the values and has as its single argument the other value from the dictionary.

## See Also

### Related Documentation

var allKeys: [Any]

A new array containing the dictionary’s keys, or an empty array if the dictionary has no entries.

func sortedArray(using: Selector) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given selector.

### Sorting Dictionaries

func keysSortedByValue(comparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values using a given comparator block.

func keysSortedByValue(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values using a given comparator block and a specified set of options.

