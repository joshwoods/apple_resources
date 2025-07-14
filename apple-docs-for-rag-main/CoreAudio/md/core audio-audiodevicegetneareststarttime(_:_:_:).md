

- Core Audio
-  AudioDeviceGetNearestStartTime(\_:\_:\_:) 

Function

# AudioDeviceGetNearestStartTime(\_:\_:\_:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+

``` source
func AudioDeviceGetNearestStartTime(
    _ inDevice: AudioObjectID,
    _ ioRequestedStartTime: UnsafeMutablePointer,
    _ inFlags: UInt32
) -> OSStatus
```

## See Also

### Functions

func AudioConvertHostTimeToNanos(UInt64) -> UInt64

func AudioConvertNanosToHostTime(UInt64) -> UInt64

func AudioDeviceCreateIOProcID(AudioObjectID, AudioDeviceIOProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;AudioDeviceIOProcID?>) -> OSStatus

func AudioDeviceCreateIOProcIDWithBlock(UnsafeMutablePointer&lt;AudioDeviceIOProcID?>, AudioObjectID, dispatch_queue_t?, AudioDeviceIOBlock) -> OSStatus

func AudioDeviceDestroyIOProcID(AudioObjectID, AudioDeviceIOProcID) -> OSStatus

func AudioDeviceGetCurrentTime(AudioObjectID, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

func AudioDeviceStart(AudioObjectID, AudioDeviceIOProcID?) -> OSStatus

func AudioDeviceStartAtTime(AudioObjectID, AudioDeviceIOProcID?, UnsafeMutablePointer&lt;AudioTimeStamp>, UInt32) -> OSStatus

func AudioDeviceStop(AudioObjectID, AudioDeviceIOProcID?) -> OSStatus

func AudioDeviceTranslateTime(AudioObjectID, UnsafePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

func AudioGetCurrentHostTime() -> UInt64

func AudioGetHostClockFrequency() -> Float64

func AudioGetHostClockMinimumTimeDelta() -> UInt32

func AudioHardwareCreateAggregateDevice(CFDictionary, UnsafeMutablePointer&lt;AudioObjectID>) -> OSStatus

func AudioHardwareDestroyAggregateDevice(AudioObjectID) -> OSStatus

