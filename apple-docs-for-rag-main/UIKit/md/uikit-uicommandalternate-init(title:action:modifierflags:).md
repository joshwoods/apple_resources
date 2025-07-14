

- UIKit
- UICommandAlternate
-  init(title:action:modifierFlags:) 

Initializer

# init(title:action:modifierFlags:)

Creates a command alternative with the specified title, action, and modifier flags.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    title: String,
    action: Selector,
    modifierFlags: UIKeyModifierFlags
)
```

## Parameters 

`title`  

The command alternative’s title.

`action`  

The action to take after a person selects the alternative command.

`modifierFlags`  

The bit mask of modifier keys that a person must press. You can use this parameter to specify which modifier keys (Command, Option, and so on) a person must also press. You may specify more than one modifier key. For a list of possible values, see UIKeyModifierFlags.

## Return Value

A command alternative object.

## See Also

### Creating a command alternative

init?(coder: NSCoder)

Creates a command alternative from data in an unarchiver.

