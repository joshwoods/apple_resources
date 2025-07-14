

- Audio Toolbox
- Audio Services
-  System Sounds 

API Collection

# System Sounds

## Topics

### Constants

var kSystemSoundID_FlashScreen: SystemSoundID

On the desktop, use this constant with the AudioServicesPlayAlertSound(_:) function to display a flash of light on the screen.

var kSystemSoundID_UserPreferredAlert: SystemSoundID

On the desktop, use this constant with the AudioServicesPlayAlertSound(_:) function to play the alert specified in the Sound preference pane.

var kUserPreferredAlert: SystemSoundID

A deprecated sound identifier.

## See Also

### Creating and Disposing of System Sound Objects

func AudioServicesCreateSystemSoundID(CFURL, UnsafeMutablePointer&lt;SystemSoundID>) -> OSStatus

Creates a system sound object.

func AudioServicesDisposeSystemSoundID(SystemSoundID) -> OSStatus

Disposes of a system sound object and associated resources.

typealias SystemSoundID

A system sound object, identified with a sound file you want to play.

Alert Sound Identifiers

Identifiers for alert sounds and alternatives to sounds, for use with the AudioServicesPlayAlertSound(_:) function.

