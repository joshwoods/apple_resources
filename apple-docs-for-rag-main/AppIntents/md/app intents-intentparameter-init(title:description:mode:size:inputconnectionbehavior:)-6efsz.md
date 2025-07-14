

- App Intents
- IntentParameter
-  init(title:description:mode:size:inputConnectionBehavior:) 

Initializer

# init(title:description:mode:size:inputConnectionBehavior:)

Creates an app intent parameter for an array with a specified size.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    mode: IntentPerson.ParameterMode = .contact,
    size: IntentCollectionSize,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, `Value.UnwrappedType` conforms to `Collection`, and `Value.ValueType` is `IntentPerson`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`mode`  

The user interface that appears when a person chooses a value for this parameter. Default value is `.contact`.

`size`  

The size of the array you specify to limit the amount of values.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

## See Also

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, mode: IntentPerson.ParameterMode, size: [IntentWidgetFamily : IntentCollectionSize], inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter for an array with a specified size per widget family.

