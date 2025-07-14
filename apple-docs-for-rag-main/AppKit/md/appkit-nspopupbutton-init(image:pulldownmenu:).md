

- AppKit
- NSPopUpButton
-  init(image:pullDownMenu:) 

Initializer

# init(image:pullDownMenu:)

Creates a standard pull-down button with a title, optional image, and menu.

macOS 10.10+

``` source
@backDeployed(before: macOS 15.0)
@MainActor @preconcurrency
convenience init(
    image: NSImage,
    pullDownMenu: NSMenu
)
```

## Parameters 

`image`  

The icon that is displayed on the button.

`pullDownMenu`  

The pull-down menu to present when interacting with the button.

## Return Value

An initialized pull-down button object.

## Discussion

Pull-down buttons created using this method have the `usesItemFromMenu` property set to `false`.

