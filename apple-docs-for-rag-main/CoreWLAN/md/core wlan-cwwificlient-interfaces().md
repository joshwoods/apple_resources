

- Core WLAN
- CWWiFiClient
-  interfaces() 

Instance Method

# interfaces()

Returns all available Wi-Fi interfaces.

macOS 10.10+

``` source
func interfaces() -> [CWInterface]?
```

## Return Value

An array of CWInterface objects, representing all of the available Wi-Fi interfaces in the system.

## See Also

### Getting Interfaces

func interface() -> CWInterface?

Returns the default Wi-Fi interface.

func interface(withName: String?) -> CWInterface?

Returns the Wi-Fi interface with the given name.

class func interfaceNames() -> [String]?

Returns the list of the names of available Wi-Fi interfaces.

Deprecated

