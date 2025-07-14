

- Audio Toolbox
-  MusicPlayerGetHostTimeForBeats(\_:\_:\_:) 

Function

# MusicPlayerGetHostTimeForBeats(\_:\_:\_:)

Gets the host time associated with a specified beat.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func MusicPlayerGetHostTimeForBeats(
    _ inPlayer: MusicPlayer,
    _ inBeats: MusicTimeStamp,
    _ outHostTime: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inPlayer`  

The music player that you are querying.

`inBeats`  

The beat number that you want the host time for.

`outHostTime`  

On output, the host time associated with the `inBeats` value.

## Return Value

A result code. This function returns an error if the player is not playing.

## Discussion

This function is valid only if the music player is playing. For converting between beats and seconds, see MusicSequenceGetSecondsForBeats(_:_:_:) and MusicSequenceGetBeatsForSeconds(_:_:_:).

## See Also

### Managing a Music Player

func NewMusicPlayer(UnsafeMutablePointer&lt;MusicPlayer?>) -> OSStatus

Creates a new music player.

func DisposeMusicPlayer(MusicPlayer) -> OSStatus

Disposes of a music player.

func MusicPlayerGetBeatsForHostTime(MusicPlayer, UInt64, UnsafeMutablePointer&lt;MusicTimeStamp>) -> OSStatus

Gets the beat number associated a specified host time.

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

typealias MusicTimeStamp

A timestamp for use by a music sequence.

