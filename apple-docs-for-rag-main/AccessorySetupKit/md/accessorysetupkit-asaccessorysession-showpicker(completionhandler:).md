

- AccessorySetupKit
- ASAccessorySession
-  showPicker(completionHandler:) 

Instance Method

# showPicker(completionHandler:)

Present a picker that shows accessories managed by a Device Discovery Extension in your app.

iOS 18.0+iPadOS 18.0+

``` source
func showPicker(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func showPicker() async throws
```

## Parameters 

`completionHandler`  

A block or closure that the picker calls when it completes the operation. The completion handler receives an NSError instance if the picker encounters an error.

## Discussion

Use this method when your app includes a DeviceDiscoveryExtension for its supported accessories. If your app doesn’t use DDE, call showPicker(for:completionHandler:) with an array of ASPickerDisplayItem instances instead.

The session’s event handler receives events when this picker displays and dismisses, as well as when the person using the app picks an accessory.

## See Also

### Displaying an accessory picker

func showPicker(for: [ASPickerDisplayItem], completionHandler: ((any Error)?) -> Void)

Present a picker that shows discovered accessories matching an array of display items.

