

- Media Player
- MPMediaPlayback
-  beginSeekingBackward() 

Instance Method

# beginSeekingBackward()

Begins seeking backward through the media content.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func beginSeekingBackward()
```

**Required**

## Discussion

Use this method to move the current playback position backward in time at an accelerated rate. Seeking begins when you call this method and continues until you call the endSeeking() method.

This method has no effect on streamed content.

## See Also

### Seeking within media

func beginSeekingForward()

Begins seeking forward through the media content.

**Required**

func endSeeking()

Ends forward and backward seeking through the media content.

**Required**

