

- AVFoundation
- AVPlayerItemOutputPullDelegate
-  outputSequenceWasFlushed(\_:) 

Instance Method

# outputSequenceWasFlushed(\_:)

Tells the delegate that a new sample sequence is commencing.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
optional func outputSequenceWasFlushed(_ output: AVPlayerItemOutput)
```

## Parameters 

`output`  

The output object that sent the message.

## Discussion

This method is called after any attempt to seek or change the playback direction of the item’s content. If you are maintaining any queued future samples, you can use your implementation of this method to discard those samples.

## See Also

### Responding to Pixel Buffer Changes

func outputMediaDataWillChange(AVPlayerItemOutput)

Tells the delegate that new samples are about to arrive.

