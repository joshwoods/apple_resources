

- Audio Toolbox
-  CAClockAddListener(\_:\_:\_:) 

Function

# CAClockAddListener(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockAddListener(
    _ inCAClock: CAClockRef,
    _ inListenerProc: CAClockListenerProc,
    _ inUserData: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Adding and Removing Listeners

func CAClockRemoveListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

typealias CAClockListenerProc

enum CAClockMessage

