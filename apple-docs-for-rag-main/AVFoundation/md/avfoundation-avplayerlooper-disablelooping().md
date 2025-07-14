

- AVFoundation
- AVPlayerLooper
-  disableLooping() 

Instance Method

# disableLooping()

Disables looping for the player queue.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func disableLooping()
```

## Discussion

The player looper will stop performing player queue operations for looping and let the current looping item replica play to the end. The player’s original actionAtItemEnd property will be restored afterwards.

## See Also

### Configuring Looping

var loopingPlayerItems: [AVPlayerItem]

An array containing replicas of the template player item used to accomplish the looping.

