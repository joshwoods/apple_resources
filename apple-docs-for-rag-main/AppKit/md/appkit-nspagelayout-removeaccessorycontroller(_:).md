

- AppKit
- NSPageLayout
-  removeAccessoryController(\_:) 

Instance Method

# removeAccessoryController(\_:)

Removes the specified controller of an accessory view.

macOS 10.5+

``` source
@MainActor
func removeAccessoryController(_ accessoryController: NSViewController)
```

## Parameters 

`accessoryController`  

The controller to remove.

## See Also

### Customizing the page setup dialog

func addAccessoryController(NSViewController)

Adds the specified controller of an accessory view to be presented in the page setup panel.

var accessoryControllers: [NSViewController]

An array of accessory view controllers belonging to the page layout panel.

