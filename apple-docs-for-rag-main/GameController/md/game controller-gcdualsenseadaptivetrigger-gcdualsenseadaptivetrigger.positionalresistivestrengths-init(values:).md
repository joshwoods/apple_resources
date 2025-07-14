

- Game Controller
- GCDualSenseAdaptiveTrigger
- GCDualSenseAdaptiveTrigger.PositionalResistiveStrengths
-  init(values:) 

Initializer

# init(values:)

Creates a resistive strengths structure with the specified strength values.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
init(values: (Float, Float, Float, Float, Float, Float, Float, Float, Float, Float))
```

## Parameters 

`values`  

The strength values for possible trigger positions. Each value is between `0` and `1`, where `0` is the minimum and `1` is the maximum strength.

## See Also

### Creating resistive strengths

init()

Creates an empty resistive strengths structure.

