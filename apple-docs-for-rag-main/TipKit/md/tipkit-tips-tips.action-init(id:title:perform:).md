

- TipKit
- Tips
- Tips.Action
-  init(id:title:perform:) 

Initializer

# init(id:title:perform:)

Creates a tip action that generates its label from a string.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    id: String? = nil,
    title: some StringProtocol,
    perform handler: @escaping () -> Void = {}
)
```

## Parameters 

`id`  

An optional identifier associated with the action. If you don’t specify a value, the system assigns the action’s `index` to this value.

`title`  

A string that describes the purpose of the tip action.

`handler`  

The function the system calls when the action triggers.

## See Also

### Initializers

init(id: String?, perform: () -> Void, () -> Text)

Creates a tip action that displays a custom label.

