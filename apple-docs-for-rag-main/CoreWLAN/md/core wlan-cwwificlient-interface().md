

- Core WLAN
- CWWiFiClient
-  interface() 

Instance Method

# interface()

Returns the default Wi-Fi interface.

macOS 10.10+

``` source
func interface() -> CWInterface?
```

## Return Value

The CWInterface object that represents the default Wi-Fi interface.

## See Also

### Getting Interfaces

func interface(withName: String?) -> CWInterface?

Returns the Wi-Fi interface with the given name.

func interfaces() -> [CWInterface]?

Returns all available Wi-Fi interfaces.

class func interfaceNames() -> [String]?

Returns the list of the names of available Wi-Fi interfaces.

Deprecated

