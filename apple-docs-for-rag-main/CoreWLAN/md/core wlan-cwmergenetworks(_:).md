

- Core WLAN
-  CWMergeNetworks(\_:) 

Function

# CWMergeNetworks(\_:)

Merges the specified set of CWNetwork objects.

macOS 10.7+

``` source
func CWMergeNetworks(_ networks: Set) -> Set
```

## Parameters 

`networks`  

The set of networks to merge.

## Discussion

Duplicate networks are defined as networks with the same SSID, security type, and BSS type. When duplicates are found, the network with the best RSSI value will remain.

## See Also

### Utility Methods

func CWKeychainCopyEAPIdentityList(UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>?) -> OSStatus

Finds and returns the available identities stored in the keychain.

