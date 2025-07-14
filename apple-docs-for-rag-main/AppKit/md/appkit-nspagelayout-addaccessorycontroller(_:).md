

- AppKit
- NSPageLayout
-  addAccessoryController(\_:) 

Instance Method

# addAccessoryController(\_:)

Adds the specified controller of an accessory view to be presented in the page setup panel.

macOS 10.5+

``` source
@MainActor
func addAccessoryController(_ accessoryController: NSViewController)
```

## Parameters 

`accessoryController`  

The controller to add.

## See Also

### Customizing the page setup dialog

func removeAccessoryController(NSViewController)

Removes the specified controller of an accessory view.

var accessoryControllers: [NSViewController]

An array of accessory view controllers belonging to the page layout panel.

