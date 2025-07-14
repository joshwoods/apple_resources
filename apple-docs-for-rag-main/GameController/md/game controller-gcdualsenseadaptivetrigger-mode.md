

- Game Controller
- GCDualSenseAdaptiveTrigger
-  mode 

Instance Property

# mode

The current configuration of the adaptive trigger.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
var mode: GCDualSenseAdaptiveTrigger.Mode { get }
```

## Discussion

There may be a delay updating this property value after you set the mode using one of the set mode methods because setting the mode requires a response from the controller.

## See Also

### Getting the mode

enum Mode

The possible modes of an adaptive trigger.

func setModeOff()

Sets the mode to off and stops any trigger effect.

