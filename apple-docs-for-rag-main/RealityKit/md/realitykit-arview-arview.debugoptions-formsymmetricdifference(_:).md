

- RealityKit
- ARView
- ARView.DebugOptions
-  formSymmetricDifference(\_:) 

Instance Method

# formSymmetricDifference(\_:)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

RealityKitSwiftiOSiPadOSMac CatalystmacOS

``` source
mutating func formSymmetricDifference(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `^` (bitwise XOR) operation on the two sets’ raw values.

## See Also

### Combining options

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

