

- AppKit
- NSPageLayout
-  accessoryControllers 

Instance Property

# accessoryControllers

An array of accessory view controllers belonging to the page layout panel.

macOS 10.5+

``` source
@MainActor
var accessoryControllers: [NSViewController] { get }
```

## Discussion

The `NSViewController` instances representing the accessory view controllers belonging to the receiver.

## See Also

### Customizing the page setup dialog

func addAccessoryController(NSViewController)

Adds the specified controller of an accessory view to be presented in the page setup panel.

func removeAccessoryController(NSViewController)

Removes the specified controller of an accessory view.

