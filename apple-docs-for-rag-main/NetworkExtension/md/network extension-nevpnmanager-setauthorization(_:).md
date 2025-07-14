

- Network Extension
- NEVPNManager
-  setAuthorization(\_:) 

Instance Method

# setAuthorization(\_:)

macOS 10.11+

``` source
func setAuthorization(_ authorization: AuthorizationRef)
```

## See Also

### Managing VPN configurations

class func shared() -> NEVPNManager

Access the single instance of `NEVPNManager`.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the VPN configuration from the Network Extension preferences.

func saveToPreferences(completionHandler: (((any Error)?) -> Void)?)

Save the VPN configuration in the Network Extension preferences.

func removeFromPreferences(completionHandler: (((any Error)?) -> Void)?)

Remove the VPN configuration from the Network Extension preferences.

