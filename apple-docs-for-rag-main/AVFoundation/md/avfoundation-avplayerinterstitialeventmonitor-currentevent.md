

- AVFoundation
- AVPlayerInterstitialEventMonitor
-  currentEvent 

Instance Property

# currentEvent

The current interstitial event.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var currentEvent: AVPlayerInterstitialEvent? { get }
```

## Discussion

The value is `nil` when primary content is playing.

## See Also

### Monitoring the current event

class let currentEventDidChangeNotification: NSNotification.Name

A notification the system posts when the monitor’s current interstitial event changes.

