

- AccessorySetupKit
- ASAccessorySession
-  removeAccessory(\_:completionHandler:) 

Instance Method

# removeAccessory(\_:completionHandler:)

Removes an accessory.

iOS 18.0+iPadOS 18.0+

``` source
func removeAccessory(
    _ accessory: ASAccessory,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func removeAccessory(_ accessory: ASAccessory) async throws
```

## Parameters 

`accessory`  

The accessory to remove.

`completionHandler`  

A block or closure that executes after the remove operation completes. The completion handler receives an NSError instance if the remove operation encounters an error.

## See Also

### Managing accessories

func renameAccessory(ASAccessory, options: ASAccessory.RenameOptions, completionHandler: ((any Error)?) -> Void)

Displays a view to rename an accessory.

struct RenameOptions

Options that affect the behavior of an accessory renaming operation.

