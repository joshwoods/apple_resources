

- Core Foundation
-  CFPlugInDynamicRegisterFunction 

Type Alias

# CFPlugInDynamicRegisterFunction

A callback which provides a plug-in the opportunity to dynamically register its types with a host.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFPlugInDynamicRegisterFunction = (CFPlugIn?) -> Void
```

## Parameters 

`plugIn`  

The `CFPlugIn` object that is engaged in dynamic registration. When using in C++, this parameter functions as a `this` pointer for the plug-in.

## Discussion

This callback is called as a plug-in is being loaded. This provides the plugin the means to dynamically register its types and factories with a plug-in’s host. The call is triggered by the presence of kCFPlugInDynamicRegistrationKey in the plug-in’s information property list.

## See Also

### Callbacks

typealias CFPlugInFactoryFunction

Callback function that a plug-in author must implement to create a plug-in instance.

typealias CFPlugInUnloadFunction

Callback function that is called, if present, just before a plug-in’s code is unloaded.

