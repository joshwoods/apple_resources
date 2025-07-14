

- Create ML
- MLDataValue
- MLDataValue.SequenceType
-  indices(of:) 

Instance Method

# indices(of:)

Returns the indices of all the elements that are equal to the given element.

Create MLSwiftiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func indices(of element: Self.Element) -> RangeSet
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`element`  

An element to look for in the collection.

## Return Value

A set of the indices of the elements that are equal to `element`.

## Discussion

For example, you can use this method to find all the places that a particular letter occurs in a string.

```
let str = "Fresh cheese in a breeze"
let allTheEs = str.indices(of: "e")
// str[allTheEs].count == 7
```

Complexity

O(*n*), where *n* is the length of the collection.

