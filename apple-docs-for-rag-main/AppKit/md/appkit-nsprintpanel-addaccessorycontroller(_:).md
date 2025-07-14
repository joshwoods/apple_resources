

- AppKit
- NSPrintPanel
-  addAccessoryController(\_:) 

Instance Method

# addAccessoryController(\_:)

Adds a custom controller to the Print panel to manage an accessory view.

macOS 10.5+

``` source
@MainActor
func addAccessoryController(_ accessoryController: any NSViewController & NSPrintPanelAccessorizing)
```

## Parameters 

`accessoryController`  

The view controller that manages your custom accessory views.

## Discussion

You can invoke this method multiple times to add multiple accessory views to the receiver’s Print panel.

The title for the accessory view is obtained from the `title` method of the view controller object.

## See Also

### Managing Accessory Views

func removeAccessoryController(any NSViewController &amp; NSPrintPanelAccessorizing)

Removes the specified controller and accessory view from the Print panel.

protocol NSPrintPanelAccessorizing

A set of methods that a Print panel object can use to get information from a printing accessory controller.

var accessoryControllers: [NSViewController]

The array of controller objects that manage the Print panel’s accessory views.

