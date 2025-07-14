

- Core WLAN
- CWInterface
-  interfaceNames() Deprecated

Type Method

# interfaceNames()

Returns the list of BSD names for WLAN interfaces available on the current system.

macOS 10.6–10.10Deprecated

``` source
class func interfaceNames() -> Set?
```

Deprecated

Use the CWWiFiClient method interfaceNames() instead.

## Return Value

An NSSet object containing NSString objects representing BSD interface names.

## Discussion

Returns an NSArray of NSString objects representing the supported WLAN BSD interface names avaliable on the current system (i.e. “en1”, “en2”). If there are no supported interfaces for the current system, then this method will return an empty NSArray object. Returns *nil* in the case of an error.

