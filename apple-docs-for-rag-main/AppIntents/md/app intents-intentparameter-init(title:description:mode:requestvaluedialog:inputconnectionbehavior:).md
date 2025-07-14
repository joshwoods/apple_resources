

- App Intents
- IntentParameter
-  init(title:description:mode:requestValueDialog:inputConnectionBehavior:) 

Initializer

# init(title:description:mode:requestValueDialog:inputConnectionBehavior:)

Creates an app intent parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    mode: IntentPerson.ParameterMode = .contact,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `IntentPerson`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`mode`  

The user interface that appears when a person chooses a value for this parameter. Default value is `.contact`.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

## See Also

### Creating an intent parameter

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, size: [IntentWidgetFamily : IntentCollectionSize], inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter for an array with a specified size per widget family.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, size: IntentCollectionSize, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter for an array with a specified size.

