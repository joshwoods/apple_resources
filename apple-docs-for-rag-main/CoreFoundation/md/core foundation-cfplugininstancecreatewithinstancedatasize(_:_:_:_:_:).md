

- Core Foundation
-  CFPlugInInstanceCreateWithInstanceDataSize(\_:\_:\_:\_:\_:) 

Function

# CFPlugInInstanceCreateWithInstanceDataSize(\_:\_:\_:\_:\_:)

Not recommended.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInInstanceCreateWithInstanceDataSize(
    _ allocator: CFAllocator!,
    _ instanceDataSize: CFIndex,
    _ deallocateInstanceFunction: CFPlugInInstanceDeallocateInstanceDataFunction!,
    _ factoryName: CFString!,
    _ getInterfaceFunction: CFPlugInInstanceGetInterfaceFunction!
) -> CFPlugInInstance!
```

## See Also

### Deprecated

func CFPlugInInstanceGetFactoryName(CFPlugInInstance!) -> CFString!

Not recommended.

func CFPlugInInstanceGetInstanceData(CFPlugInInstance!) -> UnsafeMutableRawPointer!

Not recommended.

func CFPlugInInstanceGetInterfaceFunctionTable(CFPlugInInstance!, CFString!, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>!) -> Bool

Not recommended.

func CFPlugInInstanceGetTypeID() -> CFTypeID

Not recommended.

