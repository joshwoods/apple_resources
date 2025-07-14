

- IOKit
- IOKitLib.h
-  IOServiceMatchPropertyTable(\_:\_:\_:) 

Function

# IOServiceMatchPropertyTable(\_:\_:\_:)

Match an IOService objects with matching dictionary.

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
func IOServiceMatchPropertyTable(
    _ service: io_service_t,
    _ matching: CFDictionary!,
    _ matches: UnsafeMutablePointer!
) -> kern_return_t
```

## Parameters 

`service`  

The IOService object to match.

`matching`  

A CF dictionary containing matching information. IOKitLib can construct matching dictionaries for common criteria with helper functions such as IOServiceMatching, IOServiceNameMatching, IOBSDNameMatching.

`matches`  

The boolean result is returned.

## Return Value

A kern_return_t error code.

## Discussion

This function calls the matching method of an IOService object and returns the boolean result.

## See Also

### Miscellaneous

func IOBSDNameMatching(mach_port_t, UInt32, UnsafePointer&lt;CChar>!) -> CFMutableDictionary!

Create a matching dictionary that specifies an IOService match based on BSD device name.

func IOConnectAddClient(io_connect_t, io_connect_t) -> kern_return_t

Inform a connection of a second connection.

func IOConnectAddRef(io_connect_t) -> kern_return_t

Adds a reference to the connect handle.

func IOConnectGetService(io_connect_t, UnsafeMutablePointer&lt;io_service_t>!) -> kern_return_t

Returns the IOService a connect handle was opened on.

func IOConnectMapMemory(io_connect_t, UInt32, task_port_t, UnsafeMutablePointer&lt;mach_vm_address_t>!, UnsafeMutablePointer&lt;mach_vm_size_t>!, IOOptionBits) -> kern_return_t

Map hardware or shared memory into the caller's task.

func IOConnectMapMemory64(io_connect_t, UInt32, task_port_t, UnsafeMutablePointer&lt;mach_vm_address_t>!, UnsafeMutablePointer&lt;mach_vm_size_t>!, IOOptionBits) -> kern_return_t

Map hardware or shared memory into the caller's task.

func IOConnectRelease(io_connect_t) -> kern_return_t

Remove a reference to the connect handle.

func IOConnectSetCFProperties(io_connect_t, CFTypeRef!) -> kern_return_t

Set CF container based properties on a connection.

func IOConnectSetCFProperty(io_connect_t, CFString!, CFTypeRef!) -> kern_return_t

Set a CF container based property on a connection.

func IOConnectSetNotificationPort(io_connect_t, UInt32, mach_port_t, UInt) -> kern_return_t

Set a port to receive family specific notifications.

func IOConnectUnmapMemory(io_connect_t, UInt32, task_port_t, mach_vm_address_t) -> kern_return_t

Remove a mapping made with IOConnectMapMemory.

func IOConnectUnmapMemory64(io_connect_t, UInt32, task_port_t, mach_vm_address_t) -> kern_return_t

Remove a mapping made with IOConnectMapMemory64.

func IOCreateReceivePort(UInt32, UnsafeMutablePointer&lt;mach_port_t>!) -> kern_return_t

Creates and returns a mach port suitable for receiving IOKit messages of the specified type.

func IODispatchCalloutFromMessage(UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;mach_msg_header_t>!, UnsafeMutableRawPointer!)

Dispatches callback notifications from a mach message.

func IOIteratorIsValid(io_iterator_t) -> boolean_t

Checks an iterator is still valid.

func IOIteratorNext(io_iterator_t) -> io_object_t

Returns the next object in an iteration.

func IOIteratorReset(io_iterator_t)

Resets an iteration back to the beginning.

func IOKitGetBusyState(mach_port_t, UnsafeMutablePointer&lt;UInt32>!) -> kern_return_t

Returns the busyState of all IOServices.

func IOKitWaitQuiet(mach_port_t, UnsafeMutablePointer&lt;mach_timespec_t>!) -> kern_return_t

Wait for a all IOServices' busyState to be zero.

func IOMasterPort(mach_port_t, UnsafeMutablePointer&lt;mach_port_t>!) -> kern_return_t

Returns the mach port used to initiate communication with IOKit.

func IONotificationPortCreate(mach_port_t) -> IONotificationPortRef!

Creates and returns a notification object for receiving IOKit notifications of new devices or state changes.

func IONotificationPortDestroy(IONotificationPortRef!)

Destroys a notification object created with IONotificationPortCreate. Also destroys any mach_port's or CFRunLoopSources obatined from IONotificationPortGetRunLoopSource(_:) or IONotificationPortGetMachPort(_:)

func IONotificationPortGetMachPort(IONotificationPortRef!) -> mach_port_t

Returns a mach_port to be used to listen for notifications.

func IONotificationPortGetRunLoopSource(IONotificationPortRef!) -> Unmanaged&lt;CFRunLoopSource>!

Returns a CFRunLoopSource to be used to listen for notifications.

func IONotificationPortSetDispatchQueue(IONotificationPortRef!, dispatch_queue_t!)

Sets a dispatch queue to be used to listen for notifications.

func IOObjectConformsTo(io_object_t, UnsafePointer&lt;CChar>!) -> boolean_t

Performs an OSDynamicCast operation on an IOKit object.

func IOObjectCopyBundleIdentifierForClass(CFString!) -> Unmanaged&lt;CFString>!

Return the bundle identifier of the given class.

func IOObjectCopyClass(io_object_t) -> Unmanaged&lt;CFString>!

Return the class name of an IOKit object.

func IOObjectCopySuperclassForClass(CFString!) -> Unmanaged&lt;CFString>!

Return the superclass name of the given class.

func IOObjectGetClass(io_object_t, UnsafeMutablePointer&lt;CChar>!) -> kern_return_t

Return the class name of an IOKit object.

func IOObjectGetKernelRetainCount(io_object_t) -> UInt32

Returns kernel retain count of an IOKit object.

func IOObjectGetRetainCount(io_object_t) -> UInt32

Returns kernel retain count of an IOKit object. Identical to IOObjectGetKernelRetainCount() but available prior to Mac OS 10.6.

func IOObjectGetUserRetainCount(io_object_t) -> UInt32

Returns the retain count for the current process of an IOKit object.

func IOObjectIsEqualTo(io_object_t, io_object_t) -> boolean_t

Checks two object handles to see if they represent the same kernel object.

func IOObjectRelease(io_object_t) -> kern_return_t

Releases an object handle previously returned by IOKitLib.

func IOObjectRetain(io_object_t) -> kern_return_t

Retains an object handle previously returned by IOKitLib.

func IORegistryCreateIterator(mach_port_t, UnsafePointer&lt;CChar>!, IOOptionBits, UnsafeMutablePointer&lt;io_iterator_t>!) -> kern_return_t

Create an iterator rooted at the registry root.

func IORegistryEntryCreateCFProperties(io_registry_entry_t, UnsafeMutablePointer&lt;Unmanaged&lt;CFMutableDictionary>?>!, CFAllocator!, IOOptionBits) -> kern_return_t

Create a CF dictionary representation of a registry entry's property table.

func IORegistryEntryCreateCFProperty(io_registry_entry_t, CFString!, CFAllocator!, IOOptionBits) -> Unmanaged&lt;CFTypeRef>!

Create a CF representation of a registry entry's property.

func IORegistryEntryCreateIterator(io_registry_entry_t, UnsafePointer&lt;CChar>!, IOOptionBits, UnsafeMutablePointer&lt;io_iterator_t>!) -> kern_return_t

Create an iterator rooted at a given registry entry.

func IORegistryEntryFromPath(mach_port_t, UnsafePointer&lt;CChar>!) -> io_registry_entry_t

Looks up a registry entry by path.

func IORegistryEntryGetChildEntry(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;io_registry_entry_t>!) -> kern_return_t

Returns the first child of a registry entry in a plane.

func IORegistryEntryGetChildIterator(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;io_iterator_t>!) -> kern_return_t

Returns an iterator over a registry entry’s child entries in a plane.

func IORegistryEntryGetLocationInPlane(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;CChar>!) -> kern_return_t

Returns a C-string location assigned to a registry entry, in a specified plane.

func IORegistryEntryGetName(io_registry_entry_t, UnsafeMutablePointer&lt;CChar>!) -> kern_return_t

Returns a C-string name assigned to a registry entry.

func IORegistryEntryGetNameInPlane(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;CChar>!) -> kern_return_t

Returns a C-string name assigned to a registry entry, in a specified plane.

func IORegistryEntryGetParentEntry(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;io_registry_entry_t>!) -> kern_return_t

Returns the first parent of a registry entry in a plane.

func IORegistryEntryGetParentIterator(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;io_iterator_t>!) -> kern_return_t

Returns an iterator over a registry entry’s parent entries in a plane.

func IORegistryEntryGetPath(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;CChar>!) -> kern_return_t

Create a path for a registry entry.

func IORegistryEntryGetRegistryEntryID(io_registry_entry_t, UnsafeMutablePointer&lt;UInt64>!) -> kern_return_t

Returns an ID for the registry entry that is global to all tasks.

func IORegistryEntryIDMatching(UInt64) -> CFMutableDictionary!

Create a matching dictionary that specifies an IOService match based on a registry entry ID.

func IORegistryEntryInPlane(io_registry_entry_t, UnsafePointer&lt;CChar>!) -> boolean_t

Determines if the registry entry is attached in a plane.

func IORegistryEntrySearchCFProperty(io_registry_entry_t, UnsafePointer&lt;CChar>!, CFString!, CFAllocator!, IOOptionBits) -> CFTypeRef!

Create a CF representation of a registry entry's property.

func IORegistryEntrySetCFProperties(io_registry_entry_t, CFTypeRef!) -> kern_return_t

Set CF container based properties in a registry entry.

func IORegistryEntrySetCFProperty(io_registry_entry_t, CFString!, CFTypeRef!) -> kern_return_t

Set a CF container based property in a registry entry.

func IORegistryGetRootEntry(mach_port_t) -> io_registry_entry_t

Return a handle to the registry root.

func IORegistryIteratorEnterEntry(io_iterator_t) -> kern_return_t

Recurse into the current entry in the registry iteration.

func IORegistryIteratorExitEntry(io_iterator_t) -> kern_return_t

Exits a level of recursion, restoring the current entry.

func IOServiceAddInterestNotification(IONotificationPortRef!, io_service_t, UnsafePointer&lt;CChar>!, IOServiceInterestCallback!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;io_object_t>!) -> kern_return_t

Register for notification of state changes in an IOService.

func IOServiceAddMatchingNotification(IONotificationPortRef!, UnsafePointer&lt;CChar>!, CFDictionary!, IOServiceMatchingCallback!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;io_iterator_t>!) -> kern_return_t

Look up registered IOService objects that match a matching dictionary, and install a notification request of new IOServices that match.

func IOServiceClose(io_connect_t) -> kern_return_t

Close a connection to an IOService and destroy the connect handle.

func IOServiceGetBusyState(io_service_t, UnsafeMutablePointer&lt;UInt32>!) -> kern_return_t

Returns the busyState of an IOService.

func IOServiceGetMatchingService(mach_port_t, CFDictionary!) -> io_service_t

Look up a registered IOService object that matches a matching dictionary.

func IOServiceGetMatchingServices(mach_port_t, CFDictionary!, UnsafeMutablePointer&lt;io_iterator_t>!) -> kern_return_t

Look up registered IOService objects that match a matching dictionary.

func IOServiceMatching(UnsafePointer&lt;CChar>!) -> CFMutableDictionary!

Create a matching dictionary that specifies an IOService class match.

func IOServiceNameMatching(UnsafePointer&lt;CChar>!) -> CFMutableDictionary!

Create a matching dictionary that specifies an IOService name match.

func IOServiceOpen(io_service_t, task_port_t, UInt32, UnsafeMutablePointer&lt;io_connect_t>!) -> kern_return_t

A request to create a connection to an IOService.

func IOServiceRequestProbe(io_service_t, UInt32) -> kern_return_t

A request to rescan a bus for device changes.

func IOServiceWaitQuiet(io_service_t, UnsafeMutablePointer&lt;mach_timespec_t>!) -> kern_return_t

Wait for an IOService's busyState to be zero.

