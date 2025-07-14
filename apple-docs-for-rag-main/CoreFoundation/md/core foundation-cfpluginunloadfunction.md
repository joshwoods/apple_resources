

- Core Foundation
-  CFPlugInUnloadFunction 

Type Alias

# CFPlugInUnloadFunction

Callback function that is called, if present, just before a plug-in’s code is unloaded.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFPlugInUnloadFunction = (CFPlugIn?) -> Void
```

## Parameters 

`plugIn`  

The `CFPlugIn` object that is about to be unloaded from memory. When writing in C++, this parameter functions as a `this` pointer for the plug-in.

## See Also

### Callbacks

typealias CFPlugInDynamicRegisterFunction

A callback which provides a plug-in the opportunity to dynamically register its types with a host.

typealias CFPlugInFactoryFunction

Callback function that a plug-in author must implement to create a plug-in instance.

