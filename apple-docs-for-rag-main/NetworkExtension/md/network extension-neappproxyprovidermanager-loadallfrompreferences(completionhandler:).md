

- Network Extension
- NEAppProxyProviderManager
-  loadAllFromPreferences(completionHandler:) 

Type Method

# loadAllFromPreferences(completionHandler:)

Load all of the App Proxy configurations associated with the calling app that have previously been saved to the Network Extension preferences.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class func loadAllFromPreferences(completionHandler: @escaping ([NEAppProxyProviderManager]?, (any Error)?) -> Void)
```

``` source
class func loadAllFromPreferences() async throws -> [NEAppProxyProviderManager]
```

## Parameters 

`completionHandler`  

A block that takes an NSArray of NEAppProxyProviderManager objects, and an NSError object. This block will be executed on the caller’s main thread after the load operation is complete. If no configurations exist for the calling app then the `managers` parameter will be set to nil and the error parameter will be set to nil. If an error occurred while loading the configurations, the error parameter will be set to an NSError object containing details about the error. See NEVPNError in NEVPNManager for a list of possible errors.

