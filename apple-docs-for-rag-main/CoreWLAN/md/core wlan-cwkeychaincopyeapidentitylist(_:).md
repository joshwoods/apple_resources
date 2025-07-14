

- Core WLAN
-  CWKeychainCopyEAPIdentityList(\_:) 

Function

# CWKeychainCopyEAPIdentityList(\_:)

Finds and returns the available identities stored in the keychain.

macOS 10.7+

``` source
func CWKeychainCopyEAPIdentityList(_ list: UnsafeMutablePointer?>?) -> OSStatus
```

## Return Value

An OSStatus error code which will indicate whether or not a failure occurred during execution. *errSecSuccess* indicates no error occurred.

## Discussion

If there are no available identities, this method will return *nil*.

## See Also

### Utility Methods

func CWMergeNetworks(Set&lt;CWNetwork>) -> Set&lt;CWNetwork>

Merges the specified set of CWNetwork objects.

