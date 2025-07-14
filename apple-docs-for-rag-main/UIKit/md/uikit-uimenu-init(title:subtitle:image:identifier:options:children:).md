

- UIKit
- UIMenu
-  init(title:subtitle:image:identifier:options:children:) 

Initializer

# init(title:subtitle:image:identifier:options:children:)

Creates a new menu with the specified title, subtitle, image, identifier, menu options, and child elements.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    title: String = "",
    subtitle: String? = nil,
    image: UIImage? = nil,
    identifier: UIMenu.Identifier? = nil,
    options: UIMenu.Options = [],
    children: [UIMenuElement] = []
)
```

## Parameters 

`title`  

The title of the menu.

`subtitle`  

The subtitle of the menu.

`image`  

The image to display next to the menu’s title.

`identifier`  

The unique identifier for the menu. When creating standard menus for your app, specify an appropriate constant defined in UIMenu.Identifier. For custom menus, specify a custom reverse domain name value, or specify `nil` to let this method create a unique identifier for you.

`options`  

Additional configuration options for the menu. For a list of possible values, see UIMenu.Options.

`children`  

The menu elements in the menu. Specify leaf menu elements using UIMenuElement subclasses like UIAction, UICommand, or UIKeyCommand, and specify submenus using UIMenu objects. You may specify an empty array if the menu has no child menu elements.

## See Also

### Creating a menu object

convenience init(title: String, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified values.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, preferredElementSize: UIMenu.ElementSize, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, element size, and child elements.

struct Identifier

Constants you use to identify an app’s standard menus.

struct Options

Options you use to configure a menu’s appearance.

init?(coder: NSCoder)

Creates a menu from data in an unarchiver.

