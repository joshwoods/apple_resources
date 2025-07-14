

- Network Extension
- NEVPNManager
-  removeFromPreferences(completionHandler:) 

Instance Method

# removeFromPreferences(completionHandler:)

Remove the VPN configuration from the Network Extension preferences.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func removeFromPreferences(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func removeFromPreferences() async throws
```

## Parameters 

`completionHandler`  

An optional block that takes an NSError object. If specified, this block will be executed on the caller’s main thread after the removal operation is complete. If the configuration does not exist or an error occurs while removing it, the error parameter will be set to an `NSError` object containing details about the error. See `NEVPN Errors` for a list of possible errors. If the configuration is removed successfully then the error parameter will be set to nil.

## Discussion

After the configuration is removed from the preferences the `NEVPNManager` object will still contain the configuration parameters. Calling loadFromPreferences(completionHandler:): will clear out the configuration parameters from the `NEVPNManager` object.

## See Also

### Managing VPN configurations

class func shared() -> NEVPNManager

Access the single instance of `NEVPNManager`.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the VPN configuration from the Network Extension preferences.

func saveToPreferences(completionHandler: (((any Error)?) -> Void)?)

Save the VPN configuration in the Network Extension preferences.

func setAuthorization(AuthorizationRef)

