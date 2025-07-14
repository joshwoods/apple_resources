

- Media Player
- MPMediaPlayback
-  play() 

Instance Method

# play()

Initiates playback of the current item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func play()
```

**Required**

## Mentioned in 

Playing audio using the built-in music player

## Discussion

If playback was previously paused, this method resumes playback where it left off; otherwise, this method plays the first available item, from the beginning.

If a media player isn’t prepared for playback when you call this method, this method first prepares the media player and then starts playback. To minimize playback delay, call the prepareToPlay() method before you call this method.

To receive a notification when a movie player is ready to play, register for the MPMoviePlayerLoadStateDidChangeNotification notification. You can then check load state by accessing the movie player’s loadState property.

## See Also

### Starting and stopping playback

func pause()

Pauses playback of the current item.

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

