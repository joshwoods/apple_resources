

- RealityKit
- IKComponent
- IKComponent.SolverCollection
-  removingSubranges(\_:) 

Instance Method

# removingSubranges(\_:)

Returns a collection of the elements in this collection that are not represented by the given range set.

RealityKitSwiftiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func removingSubranges(_ subranges: RangeSet) -> DiscontiguousSlice
```

## Parameters 

`subranges`  

A range set representing the indices of the elements to remove.

## Return Value

A collection of the elements that are not in `subranges`.

## Discussion

For example, this code sample finds the indices of all the vowel characters in the string, and then retrieves a collection that omits those characters.

```
let str = "The rain in Spain stays mainly in the plain."
let vowels: Set = ["a", "e", "i", "o", "u"]
let vowelIndices = str.subranges(where: { vowels.contains($0) })

let disemvoweled = str.removingSubranges(vowelIndices)
print(String(disemvoweled))
// Prints "Th rn n Spn stys mnly n th pln."
```

Complexity

O(*n*), where *n* is the length of the collection.

