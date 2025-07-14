

- UIKit
- UIMenu
-  init(coder:) 

Initializer

# init(coder:)

Creates a menu from data in an unarchiver.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Creating a menu object

convenience init(title: String, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified values.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, and child elements.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, preferredElementSize: UIMenu.ElementSize, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, element size, and child elements.

struct Identifier

Constants you use to identify an app’s standard menus.

struct Options

Options you use to configure a menu’s appearance.

