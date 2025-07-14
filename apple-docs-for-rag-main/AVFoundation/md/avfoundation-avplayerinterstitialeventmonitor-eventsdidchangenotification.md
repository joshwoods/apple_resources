

- AVFoundation
- AVPlayerInterstitialEventMonitor
-  eventsDidChangeNotification 

Type Property

# eventsDidChangeNotification

A notification the system posts when the monitor’s schedule of interstitial events changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class let eventsDidChangeNotification: NSNotification.Name
```

## See Also

### Monitoring the event schedule

var events: [AVPlayerInterstitialEvent]

The schedule of interstitial events.

