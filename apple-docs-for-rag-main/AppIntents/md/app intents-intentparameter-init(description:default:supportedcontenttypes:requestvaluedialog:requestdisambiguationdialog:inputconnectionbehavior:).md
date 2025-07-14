

- App Intents
- IntentParameter
-  init(description:default:supportedContentTypes:requestValueDialog:requestDisambiguationDialog:inputConnectionBehavior:) 

Initializer

# init(description:default:supportedContentTypes:requestValueDialog:requestDisambiguationDialog:inputConnectionBehavior:)

Creates an app intent parameter.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    supportedContentTypes: Array? = nil,
    requestValueDialog: IntentDialog? = nil,
    requestDisambiguationDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` conforms to `FileEntity`.

## Parameters 

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`supportedContentTypes`  

A list of selectable type identifiers for this parameter.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`requestDisambiguationDialog`  

A prompt that asks a person to choose among possible parameter values.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

