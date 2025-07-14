

- App Intents
- IntentParameter
-  init(title:description:kind:requestValueDialog:inputConnectionBehavior:) 

Initializer

# init(title:description:kind:requestValueDialog:inputConnectionBehavior:)

Creates an app intent parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    kind: IntentParameter.DateKind = .dateTime,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `DateComponents`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`kind`  

A value that indicates whether this parameter includes date or time.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

## See Also

### Creating an intent parameter

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, kind: IntentParameter&lt;Value>.DateKind, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, kind: IntentParameter&lt;Value>.DateKind, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, kind: IntentParameter&lt;Value>.DateKind, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

