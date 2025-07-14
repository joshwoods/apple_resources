

- Core Motion
- CMFallDetectionEvent
- CMFallDetectionEvent.UserResolution
-  CMFallDetectionEvent.UserResolution.dismissed 

Case

# CMFallDetectionEvent.UserResolution.dismissed

The user dismissed the fall event alert, but didn’t explicitly confirm or reject the event.

watchOS 7.2+

``` source
case dismissed
```

## Discussion

The user can dismiss the alert by pressing the digital crown or tapping the close button.

## See Also

### Resolutions

case confirmed

The user confirmed the event.

case rejected

The user rejected the fall event.

case unresponsive

The user didn’t respond to the fall event and the system hasn’t detected recovery motions.

