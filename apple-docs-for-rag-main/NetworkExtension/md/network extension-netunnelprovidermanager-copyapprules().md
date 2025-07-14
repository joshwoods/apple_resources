

- Network Extension
- NETunnelProviderManager
-  copyAppRules() 

Instance Method

# copyAppRules()

Returns a copy of the app rules currently set in the configuration.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func copyAppRules() -> [NEAppRule]?
```

## Return Value

An array of NEAppRule objects, or `nil` if the configuration doesn’t have any app rules.

## Mentioned in 

Routing your VPN network traffic

## Discussion

This method provides read-only access to the configuration’s app rules.

## See Also

### Managing tunnel configurations

class func loadAllFromPreferences(completionHandler: ([NETunnelProviderManager]?, (any Error)?) -> Void)

Read all of the VPN configurations created by the calling app that have previously been saved to the Network Extension preferences.

