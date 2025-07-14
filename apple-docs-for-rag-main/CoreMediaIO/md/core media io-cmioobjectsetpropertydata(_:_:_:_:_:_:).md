

- Core Media I/O
-  CMIOObjectSetPropertyData(\_:\_:\_:\_:\_:\_:) 

Function

# CMIOObjectSetPropertyData(\_:\_:\_:\_:\_:\_:)

Mac Catalyst 13.1+macOS 10.7+

``` source
func CMIOObjectSetPropertyData(
    _ objectID: CMIOObjectID,
    _ address: UnsafePointer!,
    _ qualifierDataSize: UInt32,
    _ qualifierData: UnsafeRawPointer!,
    _ dataSize: UInt32,
    _ data: UnsafeRawPointer!
) -> OSStatus
```

## See Also

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

func CMIOObjectShow(CMIOObjectID)

func CMIOStreamClockConvertHostTimeToDeviceTime(UInt64, CFTypeRef!) -> CMTime

func CMIOStreamClockCreate(CFAllocator!, CFString!, UnsafeRawPointer!, CMTime, UInt32, UInt32, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>!) -> OSStatus

