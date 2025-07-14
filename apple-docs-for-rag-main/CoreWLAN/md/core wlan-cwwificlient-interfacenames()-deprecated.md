

- Core WLAN
- CWWiFiClient
-  interfaceNames() Deprecated

Type Method

# interfaceNames()

Returns the list of the names of available Wi-Fi interfaces.

macOS 10.10–13.0Deprecated

``` source
class func interfaceNames() -> [String]?
```

Deprecated

Use -\[CWWiFiClient interfaceNames\] instead

## Return Value

An array of strings representing the names of the available Wi-Fi interfaces in the system. Any one of these names can be used with the interface(withName:) method to obtain a reference to the corresponding CWInterface instance.

## See Also

### Getting Interfaces

func interface() -> CWInterface?

Returns the default Wi-Fi interface.

func interface(withName: String?) -> CWInterface?

Returns the Wi-Fi interface with the given name.

func interfaces() -> [CWInterface]?

Returns all available Wi-Fi interfaces.

