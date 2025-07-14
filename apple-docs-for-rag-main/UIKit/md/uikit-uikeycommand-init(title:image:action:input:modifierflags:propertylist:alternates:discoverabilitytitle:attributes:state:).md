

- UIKit
- UIKeyCommand
-  init(title:image:action:input:modifierFlags:propertyList:alternates:discoverabilityTitle:attributes:state:) 

Initializer

# init(title:image:action:input:modifierFlags:propertyList:alternates:discoverabilityTitle:attributes:state:)

Creates a key command that you can use as a menu element with a shortcut key, or a shortcut key only for a view controller.

iOS 13.0+iPadOS 13.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
convenience init(
    title: String = "",
    image: UIImage? = nil,
    action: Selector,
    input: String,
    modifierFlags: UIKeyModifierFlags = [],
    propertyList: Any? = nil,
    alternates: [UICommandAlternate] = [],
    discoverabilityTitle: String? = nil,
    attributes: UIMenuElement.Attributes = [],
    state: UIMenuElement.State = .off
)
```

## Parameters 

`title`  

The title to display for the key command.

`image`  

The image to display next to the key command’s title. Only the context menu system supports the display of an image, and only when the app runs in iOS.

`action`  

The action method to execute on the responder object.

`input`  

The keys that a person must press. The string must contain one or more characters corresponding to the keys the person pressed. For a list of special characters that don’t have a textual representation, see Input strings for special keys.

`modifierFlags`  

The bit mask of modifier keys that a person must press. You can use this parameter to specify which modifier keys (Command, Option, and so on) a person must also press. You may specify more than one modifier key. For a list of possible values, see UIKeyModifierFlags.

`propertyList`  

An object that contains data to associate with the key command.

`alternates`  

An array of alternatives for the key command.

`discoverabilityTitle`  

An elaborated title that explains the purpose of the key command.

`attributes`  

The attributes indicating the style of the key command.

`state`  

The initial state of the key command.

## Discussion

After creating a key command object, you can:

- Add it as a child of a UIMenu using the menu’s init(title:image:identifier:options:children:) method.

- Add it to a view controller using the addKeyCommand(_:) method of the view controller.

- Override any responder class and return the key command directly from the responder’s keyCommands property.

## See Also

### Creating a key command object

convenience init(input: String, modifierFlags: UIKeyModifierFlags, action: Selector)

Creates a key command that matches the specified input.

init?(coder: NSCoder)

Creates a key command from data in an unarchiver.

init()

Creates a key command.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

