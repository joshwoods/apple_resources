

- Media Player
- MPMediaPlayback
-  pause() 

Instance Method

# pause()

Pauses playback of the current item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func pause()
```

**Required**

## Discussion

If the current item isn’t playing, this method has no effect. To resume playback of the current item from the pause point, call the play() method.

## See Also

### Starting and stopping playback

func play()

Initiates playback of the current item.

**Required**

func stop()

Ends playback of the current item.

**Required**

func prepareToPlay()

Prepares a media player for playback.

**Required**

var isPreparedToPlay: Bool

A Boolean value indicating whether a media player is ready to play.

**Required**

