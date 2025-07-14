

- Network Extension
- NEVPNManager
-  loadFromPreferences(completionHandler:) 

Instance Method

# loadFromPreferences(completionHandler:)

Load the VPN configuration from the Network Extension preferences.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func loadFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func loadFromPreferences() async throws
```

## Parameters 

`completionHandler`  

A block that takes an NSError object. This block will be executed on the caller’s main thread after the load operation is complete. If the configuration does not exist in the preferences or is loaded successfully, the error parameter will be nil. If an error occurred while loading the configuration, the error parameter will be set to an `NSError` object containing details about the error. See `NEVPN Errors` for a list of possible errors.

## Discussion

You must call this method at least once before calling `saveToPreferencesWithCompletionHandler:` for the first time after your app launches.

## See Also

### Managing VPN configurations

class func shared() -> NEVPNManager

Access the single instance of `NEVPNManager`.

func saveToPreferences(completionHandler: (((any Error)?) -> Void)?)

Save the VPN configuration in the Network Extension preferences.

func setAuthorization(AuthorizationRef)

func removeFromPreferences(completionHandler: (((any Error)?) -> Void)?)

Remove the VPN configuration from the Network Extension preferences.

