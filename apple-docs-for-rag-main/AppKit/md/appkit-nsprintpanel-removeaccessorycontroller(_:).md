

- AppKit
- NSPrintPanel
-  removeAccessoryController(\_:) 

Instance Method

# removeAccessoryController(\_:)

Removes the specified controller and accessory view from the Print panel.

macOS 10.5+

``` source
@MainActor
func removeAccessoryController(_ accessoryController: any NSViewController & NSPrintPanelAccessorizing)
```

## Parameters 

`accessoryController`  

The view controller to remove.

## Discussion

You use this method to remove any view controllers responsible for displaying accessory views you do not want to include in the Print panel.

## See Also

### Managing Accessory Views

func addAccessoryController(any NSViewController &amp; NSPrintPanelAccessorizing)

Adds a custom controller to the Print panel to manage an accessory view.

protocol NSPrintPanelAccessorizing

A set of methods that a Print panel object can use to get information from a printing accessory controller.

var accessoryControllers: [NSViewController]

The array of controller objects that manage the Print panel’s accessory views.

