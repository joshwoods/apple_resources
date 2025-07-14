

- Core Foundation
-  CFPlugInFactoryFunction 

Type Alias

# CFPlugInFactoryFunction

Callback function that a plug-in author must implement to create a plug-in instance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFPlugInFactoryFunction = (CFAllocator?, CFUUID?) -> UnsafeMutableRawPointer?
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`typeUUID`  

The UUID type to instantiate.

## Discussion

The plug-in author’s implementation of this function is registered with `CFPlugIn` either statically in the plug-in’s information property list, or dynamically. This function is executed as a result of a call to CFPlugInInstanceCreate(_:_:_:) by the plug-in host.

## See Also

### Callbacks

typealias CFPlugInDynamicRegisterFunction

A callback which provides a plug-in the opportunity to dynamically register its types with a host.

typealias CFPlugInUnloadFunction

Callback function that is called, if present, just before a plug-in’s code is unloaded.

