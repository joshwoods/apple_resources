

- IOKit
-  IOKit Functions 

API Collection

# IOKit Functions

## Topics

### Functions

func IOCFSerialize(CFTypeRef!, CFOptionFlags) -> CFData!

func IOCFUnserialize(UnsafePointer&lt;CChar>!, CFAllocator!, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> CFTypeRef!

func IOCFUnserializeBinary(UnsafePointer&lt;CChar>!, Int, CFAllocator!, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> CFTypeRef!

func IOCFUnserializeWithSize(UnsafePointer&lt;CChar>!, Int, CFAllocator!, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> CFTypeRef!

func IOCatalogueGetData(mach_port_t, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>!, UnsafeMutablePointer&lt;UInt32>!) -> kern_return_t

func IOCatalogueModuleLoaded(mach_port_t, UnsafeMutablePointer&lt;CChar>!) -> kern_return_t

func IOCatalogueReset(mach_port_t, UInt32) -> kern_return_t

func IOCatalogueSendData(mach_port_t, UInt32, UnsafePointer&lt;CChar>!, UInt32) -> kern_return_t

func IOCatalogueTerminate(mach_port_t, UInt32, UnsafeMutablePointer&lt;CChar>!) -> kern_return_t

func IOConnectCallAsyncMethod(mach_port_t, UInt32, mach_port_t, UnsafeMutablePointer&lt;UInt64>!, UInt32, UnsafePointer&lt;UInt64>!, UInt32, UnsafeRawPointer!, Int, UnsafeMutablePointer&lt;UInt64>!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Int>!) -> kern_return_t

func IOConnectCallAsyncScalarMethod(mach_port_t, UInt32, mach_port_t, UnsafeMutablePointer&lt;UInt64>!, UInt32, UnsafePointer&lt;UInt64>!, UInt32, UnsafeMutablePointer&lt;UInt64>!, UnsafeMutablePointer&lt;UInt32>!) -> kern_return_t

func IOConnectCallAsyncStructMethod(mach_port_t, UInt32, mach_port_t, UnsafeMutablePointer&lt;UInt64>!, UInt32, UnsafeRawPointer!, Int, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Int>!) -> kern_return_t

func IOConnectCallMethod(mach_port_t, UInt32, UnsafePointer&lt;UInt64>!, UInt32, UnsafeRawPointer!, Int, UnsafeMutablePointer&lt;UInt64>!, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Int>!) -> kern_return_t

func IOConnectCallScalarMethod(mach_port_t, UInt32, UnsafePointer&lt;UInt64>!, UInt32, UnsafeMutablePointer&lt;UInt64>!, UnsafeMutablePointer&lt;UInt32>!) -> kern_return_t

func IOConnectCallStructMethod(mach_port_t, UInt32, UnsafeRawPointer!, Int, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Int>!) -> kern_return_t

func IOConnectTrap0(io_connect_t, UInt32) -> kern_return_t

func IOConnectTrap1(io_connect_t, UInt32, UInt) -> kern_return_t

func IOConnectTrap2(io_connect_t, UInt32, UInt, UInt) -> kern_return_t

func IOConnectTrap3(io_connect_t, UInt32, UInt, UInt, UInt) -> kern_return_t

func IOConnectTrap4(io_connect_t, UInt32, UInt, UInt, UInt, UInt) -> kern_return_t

func IOConnectTrap5(io_connect_t, UInt32, UInt, UInt, UInt, UInt, UInt) -> kern_return_t

func IOConnectTrap6(io_connect_t, UInt32, UInt, UInt, UInt, UInt, UInt, UInt) -> kern_return_t

func IOCreatePlugInInterfaceForService(io_service_t, CFUUID!, CFUUID!, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;IOCFPlugInInterface>?>?>!, UnsafeMutablePointer&lt;Int32>!) -> kern_return_t

func IODestroyPlugInInterface(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;IOCFPlugInInterface>?>!) -> kern_return_t

func IOOpenFirmwarePathMatching(mach_port_t, UInt32, UnsafePointer&lt;CChar>!) -> Unmanaged&lt;CFMutableDictionary>!Deprecated

func IORegistryEntryCopyFromPath(mach_port_t, CFString!) -> io_registry_entry_t

func IORegistryEntryCopyPath(io_registry_entry_t, UnsafePointer&lt;CChar>!) -> Unmanaged&lt;CFString>!

func IORegistryEntryGetProperty(io_registry_entry_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt32>!) -> kern_return_t

func IOServiceAddNotification(mach_port_t, UnsafePointer&lt;CChar>!, CFDictionary!, mach_port_t, UInt, UnsafeMutablePointer&lt;io_iterator_t>!) -> kern_return_tDeprecated

func IOServiceAuthorize(io_service_t, UInt32) -> kern_return_t

func IOServiceOFPathToBSDName(mach_port_t, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;CChar>!) -> kern_return_tDeprecated

func IOServiceOpenAsFileDescriptor(io_service_t, Int32) -> Int32

func IOURLCreateDataAndPropertiesFromResource(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!, CFArray!, UnsafeMutablePointer&lt;Int32>!) -> Bool

func IOURLCreatePropertyFromResource(CFAllocator!, CFURL!, CFString!, UnsafeMutablePointer&lt;Int32>!) -> Unmanaged&lt;CFTypeRef>!

func IOURLWriteDataAndPropertiesToResource(CFURL!, CFData!, CFDictionary!, UnsafeMutablePointer&lt;Int32>!) -> Bool

func OSGetNotificationFromMessage(UnsafeMutablePointer&lt;mach_msg_header_t>!, UInt32, UnsafeMutablePointer&lt;UInt32>!, UnsafeMutablePointer&lt;UInt>!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!, UnsafeMutablePointer&lt;vm_size_t>!) -> kern_return_t

func IOMainPort(mach_port_t, UnsafeMutablePointer&lt;mach_port_t>!) -> kern_return_t

func IONotificationPortSetImportanceReceiver(IONotificationPortRef!) -> kern_return_t

func IORPCMessageFromMach(UnsafeMutablePointer&lt;IORPCMessageMach>!, Bool) -> UnsafeMutablePointer&lt;IORPCMessage>!

