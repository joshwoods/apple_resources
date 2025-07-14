

- Audio Toolbox
-  AudioServicesPlaySystemSound(\_:) 

Function

# AudioServicesPlaySystemSound(\_:)

Plays a system sound object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesPlaySystemSound(_ inSystemSoundID: SystemSoundID)
```

## Parameters 

`inSystemSoundID`  

The system sound to play. Before using this function, call the AudioServicesCreateSystemSoundID(_:_:) function to obtain a system sound.

## Discussion

This function plays a short sound (30 seconds or less in duration). Because sound might play for several seconds, this function is executed asynchronously. To know when a sound has finished playing, call the AudioServicesAddSystemSoundCompletion(_:_:_:_:_:) function to register a callback function.

On some iOS devices, you can pass the kSystemSoundID_Vibrate constant to invoke vibration. On other iOS devices, calling this function with that constant does nothing.

Sound files that you play using this function must be:

- No longer than 30 seconds in duration

- In linear PCM or IMA4 (IMA/ADPCM) format

- Packaged in a `.caf`, `.aif`, or `.wav` file

In addition, when you use the `AudioServicesPlaySystemSound` function:

- Sounds play at the current system audio volume, with no programmatic volume control available

- Sounds play immediately

- Looping and stereo positioning are unavailable

- Simultaneous playback is unavailable: You can play only one sound at a time

- The sound is played locally on the device speakers; it does not use audio routing.

## See Also

### Related Documentation

func AudioServicesAddSystemSoundCompletion(SystemSoundID, CFRunLoop?, CFString?, AudioServicesSystemSoundCompletionProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback function that is invoked when a specified system sound finishes playing.

func AudioServicesCreateSystemSoundID(CFURL, UnsafeMutablePointer&lt;SystemSoundID>) -> OSStatus

Creates a system sound object.

### Playing Sounds

func AudioServicesPlayAlertSoundWithCompletion(SystemSoundID, (() -> Void)?)

func AudioServicesPlaySystemSoundWithCompletion(SystemSoundID, (() -> Void)?)

func AudioServicesPlayAlertSound(SystemSoundID)

Plays a system sound as an alert.

