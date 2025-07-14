

- AccessorySetupKit
- ASAccessorySession
-  finishAuthorization(for:settings:completionHandler:) 

Instance Method

# finishAuthorization(for:settings:completionHandler:)

Finish authorization of a partially-setup accessory.

iOS 18.0+iPadOS 18.0+

``` source
func finishAuthorization(
    for accessory: ASAccessory,
    settings: ASAccessorySettings,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func finishAuthorization(
    for accessory: ASAccessory,
    settings: ASAccessorySettings
) async throws
```

## Discussion

Use this method in scenarios where an accessory has multiple wireless interfaces. For example, when an accessory has both Bluetooth and Wi-Fi, and your descriptor may only provides an SSID prefix. In this case, the Bluetooth interface onboards first and your app needs to then finish authorization with the full SSID.

## See Also

### Managing authorization

class ASAccessorySettings

Properties of an accessory.

func failAuthorization(for: ASAccessory, completionHandler: ((any Error)?) -> Void)

End authorization of a partially-configured accessory as a failure.

