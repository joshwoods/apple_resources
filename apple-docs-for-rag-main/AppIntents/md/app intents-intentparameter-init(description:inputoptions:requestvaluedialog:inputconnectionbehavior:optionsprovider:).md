

- App Intents
- IntentParameter
-  init(description:inputOptions:requestValueDialog:inputConnectionBehavior:optionsProvider:) 

Initializer

# init(description:inputOptions:requestValueDialog:inputConnectionBehavior:optionsProvider:)

Creates an app intent parameter with a list of selectable options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    inputOptions: String.IntentInputOptions? = nil,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    optionsProvider: OptionsProvider
) where OptionsProvider : DynamicOptionsProvider, OptionsProvider.DefaultValue.ValueType == String
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `String`.

## Parameters 

`description`  

Additional details about this parameter.

`inputOptions`  

An object that describes how a person can input the value.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`optionsProvider`  

An object that determines selectable options for this parameter.

