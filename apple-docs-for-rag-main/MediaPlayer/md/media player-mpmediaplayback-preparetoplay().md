

- Media Player
- MPMediaPlayback
-  prepareToPlay() 

Instance Method

# prepareToPlay()

Prepares a media player for playback.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func prepareToPlay()
```

**Required**

## Discussion

If a media player isn’t already prepared to play when you call the play() method, that method automatically calls this method. However, to minimize playback delay, call this method before you call play().

Calling this method may interrupt the media player’s audio session. For information on interruptions and how to respond to them, see Audio Session Programming Guide.

## See Also

### Starting and stopping playback

func play()

Initiates playback of the current item.

**Required**

func pause()

Pauses playback of the current item.

**Required**

func stop()

Ends playback of the current item.

**Required**

var isPreparedToPlay: Bool

A Boolean value indicating whether a media player is ready to play.

**Required**

