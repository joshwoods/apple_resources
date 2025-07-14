

- UIKit
- UICommand
-  init(coder:) 

Initializer

# init(coder:)

Creates a command from data in an unarchiver.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Creating a command

convenience init(title: String, subtitle: String?, image: UIImage?, action: Selector, propertyList: Any?, alternates: [UICommandAlternate], discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State)

Creates a command with the specified title, subtitle, image, action, property list, alternative commands, discoverability title, attributes, and state.

convenience init(title: String, image: UIImage?, action: Selector, propertyList: Any?, alternates: [UICommandAlternate], discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State)

Creates a command with the specified title, image, action, property list, alternative commands, discoverability title, attributes, and state.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

