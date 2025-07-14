

- Foundation
- Data
-  map(\_:) 

Instance Method

# map(\_:)

Returns an array containing the results of mapping the given closure over the sequence’s elements.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func map(_ transform: (Self.Element) throws(E) -> T) throws(E) -> [T] where E : Error
```

## Parameters 

`transform`  

A mapping closure. `transform` accepts an element of this sequence as its parameter and returns a transformed value of the same or of a different type.

## Return Value

An array containing the transformed elements of this sequence.

## Discussion

In this example, `map` is used first to convert the names in the array to lowercase strings and then to count their characters.

```
let cast = ["Vivien", "Marlon", "Kim", "Karl"]
let lowercaseNames = cast.map { $0.lowercased() }
// 'lowercaseNames' == ["vivien", "marlon", "kim", "karl"]
let letterCounts = cast.map { $0.count }
// 'letterCounts' == [6, 6, 3, 4]
```

