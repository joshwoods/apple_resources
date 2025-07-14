

- RealityKit
- ARView
- 
  - ARView
- ARView.Environment
- ARView.Environment.Reverb
- ARView.Environment.Reverb.Preset
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two values are not equal.

RealityKitSwiftiOSiPadOSMac CatalystmacOS

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Inequality is the inverse of equality. For any values `a` and `b`, `a != b` implies that `a == b` is `false`.

This is the default implementation of the not-equal-to operator (`!=`) for any type that conforms to `Equatable`.

## See Also

### Comparing reverb presets

static func == (ARView.Environment.Reverb.Preset, ARView.Environment.Reverb.Preset) -> Bool

Returns a Boolean value indicating whether two values are equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

