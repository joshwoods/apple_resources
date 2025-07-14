

- RealityKit
- ARView
- 
  - ARView
- ARView.Environment
- ARView.Environment.SceneUnderstanding
- ARView.Environment.SceneUnderstanding.Options
-  formUnion(\_:) 

Instance Method

# formUnion(\_:)

Inserts the elements of another set into this option set.

RealityKitSwiftiOSiPadOSMac Catalyst

``` source
mutating func formUnion(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `|` (bitwise OR) operation on the two sets’ raw values.

