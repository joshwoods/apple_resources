

- App Intents
- IntentParameterContext
-  requestConfirmation(for:dialog:view:) 

Instance Method

# requestConfirmation(for:dialog:view:)

Use `requestConfirmation` when you need to the ask user to confirm the parameter value.

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func requestConfirmation(
    for itemToConfirm: Value.ValueType,
    dialog: IntentDialog? = nil,
    @ViewBuilder view: () -> ViewType
) async throws -> Bool where ViewType : View
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Parameters 

`itemToConfirm`  

The items to be presented to the user for confirmation

`dialog`  

A custom dialog that may be used when prompting the user for the value

`view`  

A view to display when requesting confirmation.

