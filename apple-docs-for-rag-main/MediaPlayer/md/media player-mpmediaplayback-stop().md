

- Media Player
- MPMediaPlayback
-  stop() 

Instance Method

# stop()

Ends playback of the current item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func stop()
```

**Required**

## Discussion

This method stops playback of the current item and clears the playback queue. You must provide a new playback queue before playing new media items.

## See Also

### Starting and stopping playback

func play()

Initiates playback of the current item.

**Required**

func pause()

Pauses playback of the current item.

**Required**

func prepareToPlay()

Prepares a media player for playback.

**Required**

var isPreparedToPlay: Bool

A Boolean value indicating whether a media player is ready to play.

**Required**

