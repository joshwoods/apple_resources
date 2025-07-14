

- Core Foundation
-  CFPlugInCreate(\_:\_:) 

Function

# CFPlugInCreate(\_:\_:)

Creates a CFPlugIn given its URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPlugInCreate(
    _ allocator: CFAllocator!,
    _ plugInURL: CFURL!
) -> CFPlugIn!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new plug-in. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`plugInURL`  

The location of the plug-in.

## Return Value

A new plug-in. Ownership follows the The Create Rule.

## See Also

### Creating Plug-ins

func CFPlugInInstanceCreate(CFAllocator!, CFUUID!, CFUUID!) -> UnsafeMutableRawPointer!

Creates a `CFPlugIn` instance of a given type using a given factory.

