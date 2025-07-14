

- Media Player
- MPMediaPlayback
-  endSeeking() 

Instance Method

# endSeeking()

Ends forward and backward seeking through the media content.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func endSeeking()
```

**Required**

## Discussion

You must call this method to end a seeking operation begun by calling either the beginSeekingBackward() or beginSeekingForward() method. After calling this method, the player returns to the same state it was in prior to seeking. In other words, if the item was playing before seeking began, it continues playing from the new playhead position after calling this method.

This method has no effect on streamed content.

## See Also

### Seeking within media

func beginSeekingBackward()

Begins seeking backward through the media content.

**Required**

func beginSeekingForward()

Begins seeking forward through the media content.

**Required**

