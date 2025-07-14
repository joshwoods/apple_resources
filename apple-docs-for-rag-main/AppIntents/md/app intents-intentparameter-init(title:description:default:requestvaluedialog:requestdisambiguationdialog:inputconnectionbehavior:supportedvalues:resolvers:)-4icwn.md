

- App Intents
- IntentParameter
-  init(title:description:default:requestValueDialog:requestDisambiguationDialog:inputConnectionBehavior:supportedValues:resolvers:) 

Initializer

# init(title:description:default:requestValueDialog:requestDisambiguationDialog:inputConnectionBehavior:supportedValues:resolvers:)

Creates an app intent parameter that can convert the selected value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    requestValueDialog: IntentDialog? = nil,
    requestDisambiguationDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    supportedValues: [Value.ValueType] = Array(Value.ValueType.allCases),
    @ResolverSpecificationBuilder resolvers: @escaping () -> Spec
) where Spec : ResolverSpecification
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, `Value.ValueType` conforms to `AppEntity`, and `Value.ValueType` conforms to `AppEnum`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`requestDisambiguationDialog`  

A prompt that asks a person to choose among possible parameter values.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`supportedValues`  

A list of selectable options for this parameter.

`resolvers`  

An object that converts a value of another type to this parameter’s type.

