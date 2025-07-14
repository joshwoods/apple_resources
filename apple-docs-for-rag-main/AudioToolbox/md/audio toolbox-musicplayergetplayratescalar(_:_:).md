

- Audio Toolbox
-  MusicPlayerGetPlayRateScalar(\_:\_:) 

Function

# MusicPlayerGetPlayRateScalar(\_:\_:)

Gets the playback rate multiplier for a music player.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+

``` source
func MusicPlayerGetPlayRateScalar(
    _ inPlayer: MusicPlayer,
    _ outScaleRate: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inPlayer`  

The music player that you want to get the playback rate multiplier from.

`outScaleRate`  

The playback rate multiplier of the music player.

## Return Value

A result code

## Discussion

A music player’s default playback rate multiplier is 1.0.

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

typealias MusicTimeStamp

A timestamp for use by a music sequence.

