

- AccessorySetupKit
- ASAccessorySession
-  failAuthorization(for:completionHandler:) 

Instance Method

# failAuthorization(for:completionHandler:)

End authorization of a partially-configured accessory as a failure.

iOS 18.0+iPadOS 18.0+

``` source
func failAuthorization(
    for accessory: ASAccessory,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func failAuthorization(for accessory: ASAccessory) async throws
```

## See Also

### Managing authorization

func finishAuthorization(for: ASAccessory, settings: ASAccessorySettings, completionHandler: ((any Error)?) -> Void)

Finish authorization of a partially-setup accessory.

class ASAccessorySettings

Properties of an accessory.

