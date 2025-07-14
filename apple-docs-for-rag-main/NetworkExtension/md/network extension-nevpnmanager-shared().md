

- Network Extension
- NEVPNManager
-  shared() 

Type Method

# shared()

Access the single instance of `NEVPNManager`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class func shared() -> NEVPNManager
```

## Return Value

The `NEVPNManager` instance for the calling application.

## See Also

### Managing VPN configurations

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the VPN configuration from the Network Extension preferences.

func saveToPreferences(completionHandler: (((any Error)?) -> Void)?)

Save the VPN configuration in the Network Extension preferences.

func setAuthorization(AuthorizationRef)

func removeFromPreferences(completionHandler: (((any Error)?) -> Void)?)

Remove the VPN configuration from the Network Extension preferences.

