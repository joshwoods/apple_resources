

- App Intents
- IntentParameter
-  init(description:requestValueDialog:inputConnectionBehavior:optionsProvider:resolvers:) 

Initializer

# init(description:requestValueDialog:inputConnectionBehavior:optionsProvider:resolvers:)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    optionsProvider: OptionsProvider,
    @ResolverSpecificationBuilder resolvers: @escaping () -> Spec
) where Spec : ResolverSpecification, OptionsProvider : DynamicOptionsProvider, OptionsProvider.DefaultValue.ValueType == URL
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `URL`.

## Parameters 

`description`  

Additional details about this parameter.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`optionsProvider`  

An object that determines selectable options for this parameter.

`resolvers`  

An object that converts a value of another type to this parameter’s type.

