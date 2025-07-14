

- AVFoundation
- AVPlayerInterstitialEventController
-  cancelCurrentEvent(withResumptionOffset:) 

Instance Method

# cancelCurrentEvent(withResumptionOffset:)

Cancels the playback of all currently playing and scheduled interstitial events, and resumes playback of primary content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func cancelCurrentEvent(withResumptionOffset resumptionOffset: CMTime)
```

## Parameters 

`resumptionOffset`  

The time offset at which playback of the primary content resumes after interstitial playback finishes.

## Discussion

When you cancel interstitial events using this method, the resumption offset value that you specify overrides the events’s resumptionOffset value.

Note

If you call this method during the handling of coinciding interstitial events, the system cancels all events for that time. Calling this method has no impact on schedule events that have dates or times later than this event.

## See Also

### Configuring the Event Schedule

var events: [AVPlayerInterstitialEvent]!

The current schedule of interstitial events.

