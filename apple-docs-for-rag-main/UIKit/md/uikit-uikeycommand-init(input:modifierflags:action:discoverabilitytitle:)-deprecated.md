

- UIKit
- UIKeyCommand
-  init(input:modifierFlags:action:discoverabilityTitle:) Deprecated

Initializer

# init(input:modifierFlags:action:discoverabilityTitle:)

Creates a key command object that matches the specified input and has a title.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
convenience init(
    input: String,
    modifierFlags: UIKeyModifierFlags,
    action: Selector,
    discoverabilityTitle: String
)
```

Deprecated

Use init(input:modifierFlags:action:) instead.

## Parameters 

`input`  

The keys that a person must press. The string must contain one or more characters corresponding to the keys a person pressed. For a list of special characters that don’t have a textual representation, see Input strings for special keys.

`modifierFlags`  

The bit mask of modifier keys that a person must press. You can use this parameter to specify which modifier keys (Command, Option, and so on) a person must also press. You may specify more than one modifier key. For a list of possible values, see UIKeyModifierFlags.

`action`  

The action method to execute on the responder object.

`discoverabilityTitle`  

An elaborated title that explains the purpose of the key command.

## Return Value

The initialized key command object.

## Discussion

After creating a key command object, you can add it to a view controller using the addKeyCommand(_:) method of the view controller. You can also override any responder class and return the key command directly from the responder’s keyCommands property.

