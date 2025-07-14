

- Foundation
- NSMutableOrderedSet
-  sort(using:) 

Instance Method

# sort(using:)

Sorts the receiving ordered set using a given array of sort descriptors.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sort(using sortDescriptors: [NSSortDescriptor])
```

## Parameters 

`sortDescriptors`  

An array containing the `NSSortDescriptor` objects to use to sort the receiving ordered set’s contents.

## Discussion

See NSSortDescriptor for additional information.

## See Also

### Sorting Entries

func sort(comparator: (Any, Any) -> ComparisonResult)

Sorts the mutable ordered set using the comparison method specified by the comparator block.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

func sortRange(NSRange, options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the specified range of the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

