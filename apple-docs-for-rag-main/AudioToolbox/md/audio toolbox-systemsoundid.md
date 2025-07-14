

- Audio Toolbox
-  SystemSoundID 

Type Alias

# SystemSoundID

A system sound object, identified with a sound file you want to play.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias SystemSoundID = UInt32
```

## Discussion

Call the AudioServicesCreateSystemSoundID(_:_:) function to obtain a system sound object.

## See Also

### Creating and Disposing of System Sound Objects

func AudioServicesCreateSystemSoundID(CFURL, UnsafeMutablePointer&lt;SystemSoundID>) -> OSStatus

Creates a system sound object.

func AudioServicesDisposeSystemSoundID(SystemSoundID) -> OSStatus

Disposes of a system sound object and associated resources.

System Sounds

Alert Sound Identifiers

Identifiers for alert sounds and alternatives to sounds, for use with the AudioServicesPlayAlertSound(_:) function.

