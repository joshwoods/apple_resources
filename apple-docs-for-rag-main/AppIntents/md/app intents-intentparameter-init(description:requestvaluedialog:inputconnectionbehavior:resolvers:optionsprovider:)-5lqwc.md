

- App Intents
- IntentParameter
-  init(description:requestValueDialog:inputConnectionBehavior:resolvers:optionsProvider:) 

Initializer

# init(description:requestValueDialog:inputConnectionBehavior:resolvers:optionsProvider:)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    @ResolverSpecificationBuilder resolvers: @escaping () -> Spec,
    optionsProvider: OptionsProvider
) where Spec : ResolverSpecification, OptionsProvider : DynamicOptionsProvider, OptionsProvider.DefaultValue.ValueType == Measurement
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Parameters 

`description`  

Additional details about this parameter.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`resolvers`  

An object that converts a value of another type to this parameter’s type.

`optionsProvider`  

An object that determines selectable options for this parameter.

