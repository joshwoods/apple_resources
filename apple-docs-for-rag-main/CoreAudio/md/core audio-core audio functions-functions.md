

- Core Audio
-  Core Audio Functions 

API Collection

# Core Audio Functions

## Topics

### Functions

func AudioConvertHostTimeToNanos(UInt64) -> UInt64

func AudioConvertNanosToHostTime(UInt64) -> UInt64

func AudioDeviceCreateIOProcID(AudioObjectID, AudioDeviceIOProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;AudioDeviceIOProcID?>) -> OSStatus

func AudioDeviceCreateIOProcIDWithBlock(UnsafeMutablePointer&lt;AudioDeviceIOProcID?>, AudioObjectID, dispatch_queue_t?, AudioDeviceIOBlock) -> OSStatus

func AudioDeviceDestroyIOProcID(AudioObjectID, AudioDeviceIOProcID) -> OSStatus

func AudioDeviceGetCurrentTime(AudioObjectID, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

func AudioDeviceGetNearestStartTime(AudioObjectID, UnsafeMutablePointer&lt;AudioTimeStamp>, UInt32) -> OSStatus

func AudioDeviceStart(AudioObjectID, AudioDeviceIOProcID?) -> OSStatus

func AudioDeviceStartAtTime(AudioObjectID, AudioDeviceIOProcID?, UnsafeMutablePointer&lt;AudioTimeStamp>, UInt32) -> OSStatus

func AudioDeviceStop(AudioObjectID, AudioDeviceIOProcID?) -> OSStatus

func AudioDeviceTranslateTime(AudioObjectID, UnsafePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioTimeStamp>) -> OSStatus

func AudioGetCurrentHostTime() -> UInt64

func AudioGetHostClockFrequency() -> Float64

func AudioGetHostClockMinimumTimeDelta() -> UInt32

func AudioHardwareCreateAggregateDevice(CFDictionary, UnsafeMutablePointer&lt;AudioObjectID>) -> OSStatus

func AudioHardwareDestroyAggregateDevice(AudioObjectID) -> OSStatus

func AudioHardwareUnload() -> OSStatus

func AudioObjectAddPropertyListener(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, AudioObjectPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

func AudioObjectAddPropertyListenerBlock(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, dispatch_queue_t?, AudioObjectPropertyListenerBlock) -> OSStatus

func AudioObjectGetPropertyData(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioObjectGetPropertyDataSize(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioObjectHasProperty(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>) -> Bool

func AudioObjectIsPropertySettable(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

func AudioObjectRemovePropertyListener(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, AudioObjectPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

func AudioObjectRemovePropertyListenerBlock(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, dispatch_queue_t?, AudioObjectPropertyListenerBlock) -> OSStatus

func AudioObjectSetPropertyData(AudioObjectID, UnsafePointer&lt;AudioObjectPropertyAddress>, UInt32, UnsafeRawPointer?, UInt32, UnsafeRawPointer) -> OSStatus

func AudioObjectShow(AudioObjectID)

func AudioHardwareCreateProcessTap(CATapDescription!, UnsafeMutablePointer&lt;AudioObjectID>!) -> OSStatus

func AudioHardwareDestroyProcessTap(AudioObjectID) -> OSStatus

func PropertyAddress(AudioObjectPropertySelector, scope: AudioObjectPropertyScope, element: AudioObjectPropertyElement) -> AudioObjectPropertyAddress

## See Also

### Reference

Core Audio Structures

Core Audio Data Types

Core Audio Constants

Core Audio Enumerations

