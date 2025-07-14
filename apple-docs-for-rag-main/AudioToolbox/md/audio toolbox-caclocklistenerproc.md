

- Audio Toolbox
-  CAClockListenerProc 

Type Alias

# CAClockListenerProc

macOS

``` source
typealias CAClockListenerProc = (UnsafeMutableRawPointer, CAClockMessage, UnsafeRawPointer) -> Void
```

## See Also

### Adding and Removing Listeners

func CAClockAddListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

func CAClockRemoveListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

enum CAClockMessage

