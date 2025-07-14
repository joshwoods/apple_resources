

- Audio Toolbox
-  AudioServicesCreateSystemSoundID(\_:\_:) 

Function

# AudioServicesCreateSystemSoundID(\_:\_:)

Creates a system sound object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesCreateSystemSoundID(
    _ inFileURL: CFURL,
    _ outSystemSoundID: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inFileURL`  

The URL of the audio file to play.

`outSystemSoundID`  

On output, a system sound object associated with the specified audio file.

## Return Value

A result code.

## See Also

### Creating and Disposing of System Sound Objects

func AudioServicesDisposeSystemSoundID(SystemSoundID) -> OSStatus

Disposes of a system sound object and associated resources.

typealias SystemSoundID

A system sound object, identified with a sound file you want to play.

System Sounds

Alert Sound Identifiers

Identifiers for alert sounds and alternatives to sounds, for use with the AudioServicesPlayAlertSound(_:) function.

