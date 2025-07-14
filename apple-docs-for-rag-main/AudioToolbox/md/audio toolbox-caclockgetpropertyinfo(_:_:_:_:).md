

- Audio Toolbox
-  CAClockGetPropertyInfo(\_:\_:\_:\_:) 

Function

# CAClockGetPropertyInfo(\_:\_:\_:\_:)

macOS 10.4+

``` source
func CAClockGetPropertyInfo(
    _ inCAClock: CAClockRef,
    _ inPropertyID: CAClockPropertyID,
    _ outSize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## See Also

### Accessing Clock Properties

func CAClockGetProperty(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func CAClockSetProperty(CAClockRef, CAClockPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

enum CAClockPropertyID

enum CAClockSyncMode

