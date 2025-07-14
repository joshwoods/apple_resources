

- Game Controller
- GCControllerAxisInput
-  value 

Instance Property

# value

The current value of the axis.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var value: Float { get }
```

## Discussion

Often a physical controller ignores values near the neutral position called the dead zone. The GCControllerAxisInput element handles this dead zone, and other physical constraints of a hardware control, by computing a normalized value.

The normalized value ranges from `-1` to `1`. If the value is `0`, the movement is in the dead zone. A nonzero value indicates the moment is outside of the dead zone.

## See Also

### Accessing the input values

func setValue(Float)

Sets the normalized value of the axis.

