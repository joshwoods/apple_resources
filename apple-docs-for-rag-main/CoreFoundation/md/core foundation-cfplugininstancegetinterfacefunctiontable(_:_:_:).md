

- Core Foundation
-  CFPlugInInstanceGetInterfaceFunctionTable(\_:\_:\_:) 

Function

# CFPlugInInstanceGetInterfaceFunctionTable(\_:\_:\_:)

Not recommended.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInInstanceGetInterfaceFunctionTable(
    _ instance: CFPlugInInstance!,
    _ interfaceName: CFString!,
    _ ftbl: UnsafeMutablePointer!
) -> Bool
```

## See Also

### Deprecated

func CFPlugInInstanceCreateWithInstanceDataSize(CFAllocator!, CFIndex, CFPlugInInstanceDeallocateInstanceDataFunction!, CFString!, CFPlugInInstanceGetInterfaceFunction!) -> CFPlugInInstance!

Not recommended.

func CFPlugInInstanceGetFactoryName(CFPlugInInstance!) -> CFString!

Not recommended.

func CFPlugInInstanceGetInstanceData(CFPlugInInstance!) -> UnsafeMutableRawPointer!

Not recommended.

func CFPlugInInstanceGetTypeID() -> CFTypeID

Not recommended.

