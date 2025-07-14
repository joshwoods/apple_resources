

- Quartz
- QCView
-  eventForwardingMask() Deprecated

Instance Method

# eventForwardingMask()

Retrieves the mask used to filter which types of events are forwarded from the view to the composition during rendering.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func eventForwardingMask() -> Int
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The event filtering mask.

## See Also

### Setting and Getting Event Masks

func setEventForwardingMask(Int)

Sets the mask used to filter which types of events are forwarded from the view to the composition during rendering.

Deprecated

