

- RealityKit
- ARView
- 
  - ARView
- ARView.Environment
- ARView.Environment.SceneUnderstanding
- ARView.Environment.SceneUnderstanding.Options
-  formSymmetricDifference(\_:) 

Instance Method

# formSymmetricDifference(\_:)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

RealityKitSwiftiOSiPadOSMac Catalyst

``` source
mutating func formSymmetricDifference(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `^` (bitwise XOR) operation on the two sets’ raw values.

