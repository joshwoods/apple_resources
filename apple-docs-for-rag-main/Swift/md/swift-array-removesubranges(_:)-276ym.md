

- Swift
- Array
-  removeSubranges(\_:) 

Instance Method

# removeSubranges(\_:)

Removes the elements at the given indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func removeSubranges(_ subranges: RangeSet)
```

Available when `Self` conforms to `RangeReplaceableCollection`.

## Parameters 

`subranges`  

The indices of the elements to remove.

## Discussion

For example, this code sample finds the indices of all the negative numbers in the array, and then removes those values.

```
var numbers = [5, 7, -3, -8, 11, 2, -1, 6]
let negativeIndices = numbers.subranges(where: { $0 

Complexity

O(*n*), where *n* is the length of the collection.

