

- Audio Toolbox
-  AudioServicesDisposeSystemSoundID(\_:) 

Function

# AudioServicesDisposeSystemSoundID(\_:)

Disposes of a system sound object and associated resources.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesDisposeSystemSoundID(_ inSystemSoundID: SystemSoundID) -> OSStatus
```

## Parameters 

`inSystemSoundID`  

The system sound object to dispose of.

## Return Value

A result code.

## See Also

### Creating and Disposing of System Sound Objects

func AudioServicesCreateSystemSoundID(CFURL, UnsafeMutablePointer&lt;SystemSoundID>) -> OSStatus

Creates a system sound object.

typealias SystemSoundID

A system sound object, identified with a sound file you want to play.

System Sounds

Alert Sound Identifiers

Identifiers for alert sounds and alternatives to sounds, for use with the AudioServicesPlayAlertSound(_:) function.

