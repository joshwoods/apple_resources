

- PHASE
- PHASEGroupPreset
-  timeToReset 

Instance Property

# timeToReset

A duration in which the framework restores the group’s original state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var timeToReset: Double { get }
```

## Discussion

This property determines the speed of deactivation when the app calls deactivate(). The framework scales the value by unitsPerSecond.

## See Also

### Fading Between Settings

var timeToTarget: Double

A duration in which the engine fades the settings from their original value to their new value.

