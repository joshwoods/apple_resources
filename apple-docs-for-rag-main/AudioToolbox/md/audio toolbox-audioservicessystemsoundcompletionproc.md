

- Audio Toolbox
-  AudioServicesSystemSoundCompletionProc 

Type Alias

# AudioServicesSystemSoundCompletionProc

A function the system invokes when a system sound finishes playing.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioServicesSystemSoundCompletionProc = (SystemSoundID, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`ssID`  

The system sound that has finished playing.

`clientData`  

App data that you specified when registering the callback function.

## Discussion

Because a system sound may play for up to 30 seconds, the AudioServicesPlaySystemSound(_:) function executes asynchronously (that is, it returns immediately), and calls this function when the sound finishes playing. You can use this callback, for example, to help you avoid playing a second sound while a first sound is still playing.

## See Also

### Adding and Removing System Sound Callbacks

func AudioServicesAddSystemSoundCompletion(SystemSoundID, CFRunLoop?, CFString?, AudioServicesSystemSoundCompletionProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback function that is invoked when a specified system sound finishes playing.

func AudioServicesRemoveSystemSoundCompletion(SystemSoundID)

Unregisters any completion callback functions that were registered for a specified system sound.

