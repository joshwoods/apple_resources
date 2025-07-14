

- TipKit
- Tips
- Tips.Action
-  init(id:perform:\_:) 

Initializer

# init(id:perform:\_:)

Creates a tip action that displays a custom label.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    id: String? = nil,
    perform handler: @escaping () -> Void = {},
    _ label: @escaping () -> Text
)
```

## Parameters 

`id`  

An optional identifier associated with the action. If you don’t specify a value, the system assigns the action’s `index` to this value.

`handler`  

The function the system calls when the action triggers.

`label`  

A view that describes the purpose of the tip action.

## See Also

### Initializers

init(id: String?, title: some StringProtocol, perform: () -> Void)

Creates a tip action that generates its label from a string.

