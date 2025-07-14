

- Network Extension
- NEHotspotConfigurationManager
-  joinAccessoryHotspot(\_:passphrase:completionHandler:) 

Instance Method

# joinAccessoryHotspot(\_:passphrase:completionHandler:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
func joinAccessoryHotspot(
    _ accessory: ASAccessory,
    passphrase: String,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func joinAccessoryHotspot(
    _ accessory: ASAccessory,
    passphrase: String
) async throws
```

