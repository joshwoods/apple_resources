

- Foundation
- NSNotification
- NSNotification.Name
-  MPMovieDurationAvailable Deprecated

Type Property

# MPMovieDurationAvailable

Posted when the duration of a movie has been determined. There is no `userInfo` dictionary.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–9.0Deprecated

``` source
static let MPMovieDurationAvailable: NSNotification.Name
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

To retrieve the duration of a movie, access the movie player’s duration property. The movie player whose state has changed is available as the object associated with the notification.

## See Also

### MediaPlayer

static let MPMusicPlayerControllerQueueDidChange: NSNotification.Name

Indicates the music player’s queue changed.

static let MPMediaLibraryDidChange: NSNotification.Name

Indicates the media library has changed.

static let MPMediaPlaybackIsPreparedToPlayDidChange: NSNotification.Name

Indicates that the prepared to play status of the media player has changed.

Deprecated

static let MPMusicPlayerControllerNowPlayingItemDidChange: NSNotification.Name

Posted when the currently playing media item has changed.

static let MPMusicPlayerControllerPlaybackStateDidChange: NSNotification.Name

Posted when the playback state changes programmatically or by user action.

static let MPMusicPlayerControllerVolumeDidChange: NSNotification.Name

Posted when the audio playback volume for the music player has changed.

static let MPMovieMediaTypesAvailable: NSNotification.Name

Posted when the available media types in a movie are determined. There is no `userInfo` dictionary.

Deprecated

static let MPMovieNaturalSizeAvailable: NSNotification.Name

Posted when the natural frame size of a movie is first determined or subsequently changes. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerDidEnterFullscreen: NSNotification.Name

Posted when a movie player has entered full-screen mode. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerDidExitFullscreen: NSNotification.Name

Posted when a movie player has exited full-screen mode. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerIsAirPlayVideoActiveDidChange: NSNotification.Name

Posted when a movie player has started or ended playing a movie via AirPlay. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerLoadStateDidChange: NSNotification.Name

Posted when a movie player’s network buffering state has changed. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerNowPlayingMovieDidChange: NSNotification.Name

Posted when the currently playing movie has changed. There is no `userInfo` dictionary.

Deprecated

static let MPMoviePlayerPlaybackDidFinish: NSNotification.Name

Posted when a movie has finished playing. The `userInfo` dictionary of this notification contains the MPMoviePlayerPlaybackDidFinishReasonUserInfoKey key, which indicates the reason that playback finished. This notification is also sent when playback fails because of an error.

Deprecated

static let MPMoviePlayerPlaybackStateDidChange: NSNotification.Name

Posted when a movie player’s playback state has changed. There is no `userInfo` dictionary.

Deprecated

