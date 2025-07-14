

- AppKit
- NSPrintPanel
-  accessoryControllers 

Instance Property

# accessoryControllers

The array of controller objects that manage the Print panel’s accessory views.

macOS 10.5+

``` source
@MainActor
var accessoryControllers: [NSViewController] { get }
```

## Discussion

This property contains an array of NSViewController objects, each of which represents an accessory view added using the addAccessoryController(_:) method.

## See Also

### Managing Accessory Views

func addAccessoryController(any NSViewController &amp; NSPrintPanelAccessorizing)

Adds a custom controller to the Print panel to manage an accessory view.

func removeAccessoryController(any NSViewController &amp; NSPrintPanelAccessorizing)

Removes the specified controller and accessory view from the Print panel.

protocol NSPrintPanelAccessorizing

A set of methods that a Print panel object can use to get information from a printing accessory controller.

