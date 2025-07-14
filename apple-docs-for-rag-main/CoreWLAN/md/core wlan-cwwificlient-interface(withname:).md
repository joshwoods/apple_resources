

- Core WLAN
- CWWiFiClient
-  interface(withName:) 

Instance Method

# interface(withName:)

Returns the Wi-Fi interface with the given name.

macOS 10.10+

``` source
func interface(withName interfaceName: String?) -> CWInterface?
```

## Parameters 

`interfaceName`  

The name of an available Wi-Fi interface. Use the interfaceNames() class method to obtain a list of valid interface names.

## Return Value

The CWInterface object bound to the given interface name, or the default interface if no name is specified.

## See Also

### Getting Interfaces

func interface() -> CWInterface?

Returns the default Wi-Fi interface.

func interfaces() -> [CWInterface]?

Returns all available Wi-Fi interfaces.

class func interfaceNames() -> [String]?

Returns the list of the names of available Wi-Fi interfaces.

Deprecated

