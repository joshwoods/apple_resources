

- AppKit
- NSPopUpButton
-  init(title:image:pullDownMenu:) 

Initializer

# init(title:image:pullDownMenu:)

Creates a standard pull-down button with a title, optional image, and menu.

macOS 10.10+

``` source
@backDeployed(before: macOS 15.0)
@MainActor @preconcurrency
convenience init(
    title: String,
    image: NSImage? = nil,
    pullDownMenu: NSMenu
)
```

## Parameters 

`title`  

The localized title string that is displayed on the button.

`image`  

The icon that is displayed on the button.

`pullDownMenu`  

The pull-down menu to present when interacting with the button.

## Return Value

An initialized pull-down button object.

## Discussion

Pull-down buttons created using this method have the `usesItemFromMenu` property set to `false`.

