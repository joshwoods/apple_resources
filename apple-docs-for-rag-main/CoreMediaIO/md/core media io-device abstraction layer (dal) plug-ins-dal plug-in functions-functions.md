

- Core Media I/O
- Device Abstraction Layer (DAL) Plug-Ins
-  DAL plug-in functions 

API Collection

# DAL plug-in functions

## Topics

### Functions

func CMIODeviceProcessAVCCommand(CMIODeviceID, UnsafeMutablePointer&lt;CMIODeviceAVCCommand>!) -> OSStatus

func CMIODeviceProcessRS422Command(CMIODeviceID, UnsafeMutablePointer&lt;CMIODeviceRS422Command>!) -> OSStatus

func CMIODeviceStartStream(CMIODeviceID, CMIOStreamID) -> OSStatus

func CMIODeviceStopStream(CMIODeviceID, CMIOStreamID) -> OSStatus

func CMIOObjectAddPropertyListener(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, CMIOObjectPropertyListenerProc!, UnsafeMutableRawPointer!) -> OSStatus

func CMIOObjectAddPropertyListenerBlock(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, dispatch_queue_t!, CMIOObjectPropertyListenerBlock!) -> OSStatus

func CMIOObjectGetPropertyData(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, UInt32, UnsafeRawPointer!, UInt32, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutableRawPointer!) -> OSStatus

func CMIOObjectGetPropertyDataSize(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, UInt32, UnsafeRawPointer!, UnsafeMutablePointer&lt;UInt32>!) -> OSStatus

func CMIOObjectHasProperty(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!) -> Bool

func CMIOObjectIsPropertySettable(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> OSStatus

func CMIOObjectRemovePropertyListener(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, CMIOObjectPropertyListenerProc!, UnsafeMutableRawPointer!) -> OSStatus

func CMIOObjectRemovePropertyListenerBlock(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, dispatch_queue_t!, CMIOObjectPropertyListenerBlock!) -> OSStatus

func CMIOObjectSetPropertyData(CMIOObjectID, UnsafePointer&lt;CMIOObjectPropertyAddress>!, UInt32, UnsafeRawPointer!, UInt32, UnsafeRawPointer!) -> OSStatus

func CMIOObjectShow(CMIOObjectID)

func CMIOStreamClockConvertHostTimeToDeviceTime(UInt64, CFTypeRef!) -> CMTime

func CMIOStreamClockCreate(CFAllocator!, CFString!, UnsafeRawPointer!, CMTime, UInt32, UInt32, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>!) -> OSStatus

func CMIOStreamClockInvalidate(CFTypeRef!) -> OSStatus

func CMIOStreamClockPostTimingEvent(CMTime, UInt64, Bool, CFTypeRef!) -> OSStatus

func CMIOStreamCopyBufferQueue(CMIOStreamID, CMIODeviceStreamQueueAlteredProc!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CMSimpleQueue>?>!) -> OSStatus

func CMIOStreamDeckCueTo(CMIOStreamID, UInt64, Bool) -> OSStatus

func CMIOStreamDeckJog(CMIOStreamID, Int32) -> OSStatus

func CMIOStreamDeckPlay(CMIOStreamID) -> OSStatus

func CMIOStreamDeckStop(CMIOStreamID) -> OSStatus

## See Also

### Reference

DAL plug-in structures

DAL plug-in enumerations

DAL plug-in data types

DAL plug-in errors

