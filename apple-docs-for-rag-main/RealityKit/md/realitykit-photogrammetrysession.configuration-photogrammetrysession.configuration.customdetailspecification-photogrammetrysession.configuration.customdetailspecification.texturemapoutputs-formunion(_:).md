

- RealityKit
- PhotogrammetrySession
- 
  - PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
- PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs
-  formUnion(\_:) 

Instance Method

# formUnion(\_:)

Inserts the elements of another set into this option set.

RealityKitSwiftMac CatalystmacOS

``` source
mutating func formUnion(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `|` (bitwise OR) operation on the two sets’ raw values.

