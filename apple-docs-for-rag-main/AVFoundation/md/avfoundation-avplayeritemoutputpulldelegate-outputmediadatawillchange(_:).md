

- AVFoundation
- AVPlayerItemOutputPullDelegate
-  outputMediaDataWillChange(\_:) 

Instance Method

# outputMediaDataWillChange(\_:)

Tells the delegate that new samples are about to arrive.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
optional func outputMediaDataWillChange(_ sender: AVPlayerItemOutput)
```

## Parameters 

`sender`  

The output object that sent the message.

## Discussion

You can use this method to prepare for any new sample data. This method is called at some point after a call to your video output object’s `requestNotificationOfMediaDataChangeWithAdvanceInterval:` method.

## See Also

### Responding to Pixel Buffer Changes

func outputSequenceWasFlushed(AVPlayerItemOutput)

Tells the delegate that a new sample sequence is commencing.

