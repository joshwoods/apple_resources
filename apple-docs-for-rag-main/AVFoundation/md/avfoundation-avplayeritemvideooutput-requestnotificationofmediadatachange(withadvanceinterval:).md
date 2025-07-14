

- AVFoundation
- AVPlayerItemVideoOutput
-  requestNotificationOfMediaDataChange(withAdvanceInterval:) 

Instance Method

# requestNotificationOfMediaDataChange(withAdvanceInterval:)

Tells the receiver that the video out put client is entering a quiescent state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func requestNotificationOfMediaDataChange(withAdvanceInterval interval: TimeInterval)
```

## Parameters 

`interval`  

The amount of time to wait before notifying the delegate of the media change.

## Discussion

Call this method before you suspend your use of a CVDisplayLink type or a CADisplayLink object. After the interval expires, the video output object notifies its delegate that it should resume the display link. If the interval value you specify is large, the delegate is notified as soon as possible rather than waiting.

Do not call this method repeatedly to force the delegate to be notified for each sample.

