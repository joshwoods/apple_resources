

- Network Extension
- NETunnelProviderManager
-  loadAllFromPreferences(completionHandler:) 

Type Method

# loadAllFromPreferences(completionHandler:)

Read all of the VPN configurations created by the calling app that have previously been saved to the Network Extension preferences.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class func loadAllFromPreferences(completionHandler: @escaping ([NETunnelProviderManager]?, (any Error)?) -> Void)
```

``` source
class func loadAllFromPreferences() async throws -> [NETunnelProviderManager]
```

## Parameters 

`completionHandler`  

A block that takes an NSArray of `NETunnelProviderManager` objects, and an NSError object. This block will be executed on the caller’s main thread after the load operation is complete. If no configurations exist for the calling app then the `managers` parameter will be set to nil and the error parameter will be set to nil. If an error occurred while loading the configurations, the error parameter will be set to an NSError object containing details about the error. See NEVPNManager for a list of possible errors.

## See Also

### Managing tunnel configurations

func copyAppRules() -> [NEAppRule]?

Returns a copy of the app rules currently set in the configuration.

