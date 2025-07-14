

- UIKit
- UIKeyCommand
-  init() 

Initializer

# init()

Creates a key command.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init()
```

## See Also

### Creating a key command object

convenience init(title: String, image: UIImage?, action: Selector, input: String, modifierFlags: UIKeyModifierFlags, propertyList: Any?, alternates: [UICommandAlternate], discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State)

Creates a key command that you can use as a menu element with a shortcut key, or a shortcut key only for a view controller.

convenience init(input: String, modifierFlags: UIKeyModifierFlags, action: Selector)

Creates a key command that matches the specified input.

init?(coder: NSCoder)

Creates a key command from data in an unarchiver.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

