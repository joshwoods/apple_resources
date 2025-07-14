

- Core WLAN
-  CWKeychainDeleteWiFiPassword(\_:\_:) 

Function

# CWKeychainDeleteWiFiPassword(\_:\_:)

Deletes the password for the SSID and keychain domain you specify.

macOS 10.9+

``` source
func CWKeychainDeleteWiFiPassword(
    _ domain: CWKeychainDomain,
    _ ssid: Data
) -> OSStatus
```

## See Also

### Functions

func CWKeychainCopyWiFiEAPIdentity(CWKeychainDomain, Data, UnsafeMutablePointer&lt;Unmanaged&lt;SecIdentity>?>?) -> OSStatus

Finds and returns the identity stored for the SSID and keychain domain you specify.

func CWKeychainDeleteWiFiEAPUsernameAndPassword(CWKeychainDomain, Data) -> OSStatus

Deletes the 802.1X username and password for the SSID and keychain domain you specify.

func CWKeychainFindWiFiEAPUsernameAndPassword(CWKeychainDomain, Data, AutoreleasingUnsafeMutablePointer&lt;NSString?>?, AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> OSStatus

Finds and returns the 802.1X username and password stored for the SSID and keychain domain you specify.

func CWKeychainFindWiFiPassword(CWKeychainDomain, Data, AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> OSStatus

Finds and returns, by reference, the password for the SSID and keychain domain you specify.

func CWKeychainSetWiFiEAPIdentity(CWKeychainDomain, Data, SecIdentity?) -> OSStatus

Associates an identity to the SSID and keychain domain you specify.

func CWKeychainSetWiFiEAPUsernameAndPassword(CWKeychainDomain, Data, String?, String?) -> OSStatus

Sets the 802.1X username and password for the SSID and keychain domain you specify.

func CWKeychainSetWiFiPassword(CWKeychainDomain, Data, String) -> OSStatus

Sets the Wi-Fi network keychain password for the SSID and keychain domain you specify.

