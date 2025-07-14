

- Network Extension
- NEVPNManager
-  saveToPreferences(completionHandler:) 

Instance Method

# saveToPreferences(completionHandler:)

Save the VPN configuration in the Network Extension preferences.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func saveToPreferences(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func saveToPreferences() async throws
```

## Parameters 

`completionHandler`  

An optional block that takes an NSError object. If specified, this block will be executed on the caller’s main thread after the save operation is complete. If the configuration could not be saved to the preferences, the error parameter will be set to an `NSError` object containing details about the error. See `NEVPN Errors` for a list of possible errors. If the configuration is saved successfully then the error parameter will be set to nil.

## Discussion

You must call loadFromPreferences(completionHandler:): at least once before calling this method the first time after your app launches.

## See Also

### Related Documentation

class NEVPNManager

An object to create and manage a Personal VPN configuration.

### Managing VPN configurations

class func shared() -> NEVPNManager

Access the single instance of `NEVPNManager`.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the VPN configuration from the Network Extension preferences.

func setAuthorization(AuthorizationRef)

func removeFromPreferences(completionHandler: (((any Error)?) -> Void)?)

Remove the VPN configuration from the Network Extension preferences.

