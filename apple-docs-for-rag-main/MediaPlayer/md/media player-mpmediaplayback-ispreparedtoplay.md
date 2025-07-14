

- Media Player
- MPMediaPlayback
-  isPreparedToPlay 

Instance Property

# isPreparedToPlay

A Boolean value indicating whether a media player is ready to play.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
var isPreparedToPlay: Bool { get }
```

**Required**

## Discussion

When set to true, the media player is ready to begin playing the queued media items.

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

func prepareToPlay()

Prepares a media player for playback.

**Required**

