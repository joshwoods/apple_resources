

- RealityKit
- PhysicsJoints
-  removeSubranges(\_:) 

Instance Method

# removeSubranges(\_:)

Removes the elements at the given indices.

RealityKitSwiftiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func removeSubranges(_ subranges: RangeSet)
```

## Parameters 

`subranges`  

The indices of the elements to remove.

## Discussion

For example, this code sample finds the indices of all the vowel characters in the string, and then removes those characters.

```
var str = "The rain in Spain stays mainly in the plain."
let vowels: Set = ["a", "e", "i", "o", "u"]
let vowelIndices = str.subranges(where: { vowels.contains($0) })

str.removeSubranges(vowelIndices)
// str == "Th rn n Spn stys mnly n th pln."
```

Complexity

O(*n*), where *n* is the length of the collection.

