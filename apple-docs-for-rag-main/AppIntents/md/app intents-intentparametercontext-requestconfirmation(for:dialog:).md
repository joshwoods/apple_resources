

- App Intents
- IntentParameterContext
-  requestConfirmation(for:dialog:) 

Instance Method

# requestConfirmation(for:dialog:)

Use `requestConfirmation` when you need to the ask user to confirm the parameter value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func requestConfirmation(
    for itemToConfirm: Value.ValueType,
    dialog: IntentDialog? = nil
) async throws -> Bool
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Parameters 

`itemToConfirm`  

The items to be presented to the user for confirmation

`dialog`  

A custom dialog that may be used when prompting the user for the value

## Return Value

Whether or not the user confirmed the value

