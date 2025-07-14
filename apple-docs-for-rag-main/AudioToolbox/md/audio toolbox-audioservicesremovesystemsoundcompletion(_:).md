

- Audio Toolbox
-  AudioServicesRemoveSystemSoundCompletion(\_:) 

Function

# AudioServicesRemoveSystemSoundCompletion(\_:)

Unregisters any completion callback functions that were registered for a specified system sound.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesRemoveSystemSoundCompletion(_ inSystemSoundID: SystemSoundID)
```

## Parameters 

`inSystemSoundID`  

The system sound for which callback functions should be removed.

## See Also

### Adding and Removing System Sound Callbacks

func AudioServicesAddSystemSoundCompletion(SystemSoundID, CFRunLoop?, CFString?, AudioServicesSystemSoundCompletionProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback function that is invoked when a specified system sound finishes playing.

typealias AudioServicesSystemSoundCompletionProc

A function the system invokes when a system sound finishes playing.

