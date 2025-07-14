

- Core WLAN
- CWInterface
-  init(name:) Deprecated

Initializer

# init(name:)

An instance method for obtaining an CWInterface object.

macOS 10.6–10.10Deprecated

``` source
convenience init(name: String?)
```

Deprecated

This method relies on direct access to system sockets, and therefore cannot be used in a sandboxed app. Use the interface(withName:) instance method of CWWiFiClient instead.

## Parameters 

`name`  

An NSString representing the BSD name of a WLAN interface.

## Return Value

An CWInterface object configured to control the named CoreWLAN interface.

## Discussion

The interface name must be in the BSD name form (e.g. “en1”), and can be passed in explicitly or derived from the call to *+(NSString \*)supportedInterfaces*. If *name* is *nil*, the method returns an CWInterface object for the primary interface. This method is the designated initializer for the CWInterface class.

## See Also

### Getting an interface

init(interfaceName: String?)

Convenience method for getting an CWInterface object with the specified name.

Deprecated

