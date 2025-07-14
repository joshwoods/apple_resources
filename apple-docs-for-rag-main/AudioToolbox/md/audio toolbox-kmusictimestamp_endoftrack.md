

- Audio Toolbox
-  kMusicTimeStamp_EndOfTrack 

Global Variable

# kMusicTimeStamp_EndOfTrack

Indicates a time immediately beyond the last music event in a music track. Use this value when selecting all music events starting at a designated time and extending to, and including, the last event in a track. Also use this value to position an iterator for moving backward through a track, from the end to the start. See also NewMusicEventIterator(_:_:) and MusicEventIteratorSeek(_:_:).

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kMusicTimeStamp_EndOfTrack: Double { get }
```

## See Also

### Managing a Music Player

func NewMusicPlayer(UnsafeMutablePointer&lt;MusicPlayer?>) -> OSStatus

Creates a new music player.

func DisposeMusicPlayer(MusicPlayer) -> OSStatus

Disposes of a music player.

func MusicPlayerGetBeatsForHostTime(MusicPlayer, UInt64, UnsafeMutablePointer&lt;MusicTimeStamp>) -> OSStatus

Gets the beat number associated a specified host time.

func MusicPlayerGetHostTimeForBeats(MusicPlayer, MusicTimeStamp, UnsafeMutablePointer&lt;UInt64>) -> OSStatus

Gets the host time associated with a specified beat.

func MusicPlayerGetPlayRateScalar(MusicPlayer, UnsafeMutablePointer&lt;Float64>) -> OSStatus

Gets the playback rate multiplier for a music player.

func MusicPlayerGetSequence(MusicPlayer, UnsafeMutablePointer&lt;MusicSequence?>) -> OSStatus

Gets the music sequence associated with a music player.

func MusicPlayerGetTime(MusicPlayer, UnsafeMutablePointer&lt;MusicTimeStamp>) -> OSStatus

Gets the playback point for a music player, in beats.

func MusicPlayerIsPlaying(MusicPlayer, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether or not a music player is playing.

func MusicPlayerPreroll(MusicPlayer) -> OSStatus

Prepares a music player to play.

func MusicPlayerSetPlayRateScalar(MusicPlayer, Float64) -> OSStatus

Sets a playback rate multiplier for a music player.

func MusicPlayerSetSequence(MusicPlayer, MusicSequence?) -> OSStatus

Sets the music sequence for the music player to play.

func MusicPlayerSetTime(MusicPlayer, MusicTimeStamp) -> OSStatus

Sets the playback point for a music player, in beats.

func MusicPlayerStart(MusicPlayer) -> OSStatus

Starts playback of a music player.

func MusicPlayerStop(MusicPlayer) -> OSStatus

Stops playback of a music player.

typealias MusicPlayer

A music player plays a music sequence (of type `MusicSequence`).

