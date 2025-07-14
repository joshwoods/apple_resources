

- Audio Toolbox
-  CAClockRemoveListener(\_:\_:\_:) 

Function

# CAClockRemoveListener(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockRemoveListener(
    _ inCAClock: CAClockRef,
    _ inListenerProc: CAClockListenerProc,
    _ inUserData: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Adding and Removing Listeners

func CAClockAddListener(CAClockRef, CAClockListenerProc, UnsafeMutableRawPointer) -> OSStatus

typealias CAClockListenerProc

enum CAClockMessage

