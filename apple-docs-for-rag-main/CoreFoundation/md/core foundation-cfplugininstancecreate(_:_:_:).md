

- Core Foundation
-  CFPlugInInstanceCreate(\_:\_:\_:) 

Function

# CFPlugInInstanceCreate(\_:\_:\_:)

Creates a `CFPlugIn` instance of a given type using a given factory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInInstanceCreate(
    _ allocator: CFAllocator!,
    _ factoryUUID: CFUUID!,
    _ typeUUID: CFUUID!
) -> UnsafeMutableRawPointer!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`factoryUUID`  

The UUID representing the factory function to use to create a plug-in of the given type.

`typeUUID`  

The UUID type.

## Return Value

Returns the IUnknown interface for the new plug-in.

## Discussion

The plug-in host uses this function to create an instance of the given type. Unless the plug-in is using dynamic registration, this function causes the plug-in’s code to be loaded into memory.

## See Also

### Creating Plug-ins

func CFPlugInCreate(CFAllocator!, CFURL!) -> CFPlugIn!

Creates a CFPlugIn given its URL.

