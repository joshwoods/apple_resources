

- AccessorySetupKit
- ASAccessorySession
-  renameAccessory(\_:options:completionHandler:) 

Instance Method

# renameAccessory(\_:options:completionHandler:)

Displays a view to rename an accessory.

iOS 18.0+iPadOS 18.0+

``` source
func renameAccessory(
    _ accessory: ASAccessory,
    options renameOptions: ASAccessory.RenameOptions = [],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func renameAccessory(
    _ accessory: ASAccessory,
    options renameOptions: ASAccessory.RenameOptions = []
) async throws
```

## Parameters 

`accessory`  

The accessory to rename.

`renameOptions`  

Options that affect the behavior of the rename operation.

`completionHandler`  

A block or closure that executes after the rename operation completes. The completion handler receives an NSError instance if the rename operation encounters an error.

## Discussion

To rename a Wi-Fi SSID with this method, use the option ssid.

## See Also

### Managing accessories

struct RenameOptions

Options that affect the behavior of an accessory renaming operation.

func removeAccessory(ASAccessory, completionHandler: ((any Error)?) -> Void)

Removes an accessory.

