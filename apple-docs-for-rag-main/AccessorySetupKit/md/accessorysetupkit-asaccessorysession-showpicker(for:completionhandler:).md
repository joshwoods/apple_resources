

- AccessorySetupKit
- ASAccessorySession
-  showPicker(for:completionHandler:) 

Instance Method

# showPicker(for:completionHandler:)

Present a picker that shows discovered accessories matching an array of display items.

iOS 18.0+iPadOS 18.0+

``` source
func showPicker(
    for displayItems: [ASPickerDisplayItem],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func showPicker(for displayItems: [ASPickerDisplayItem]) async throws
```

## Parameters 

`displayItems`  

An array of ASPickerDisplayItem instances describing accessories your app can set up. The picker displays only discovered accessories that match the properties of items in this array.

`completionHandler`  

A block or closure that the picker calls when it completes the operation. The completion handler receives an NSError instance if the picker encounters an error.

## Mentioned in 

Discovering and configuring accessories

## Discussion

The session’s event handler receives events when this picker displays and dismisses, as well as when the person using the app picks an accessory.

To migrate previously-configured accessories to AccessorySetupKit, add instances of ASMigrationDisplayItem to the `displayItems` array.

## See Also

### Displaying an accessory picker

func showPicker(completionHandler: ((any Error)?) -> Void)

Present a picker that shows accessories managed by a Device Discovery Extension in your app.

