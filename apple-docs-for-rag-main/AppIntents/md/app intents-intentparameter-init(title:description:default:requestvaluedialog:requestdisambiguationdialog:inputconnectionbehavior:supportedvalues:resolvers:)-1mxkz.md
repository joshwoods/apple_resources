

- App Intents
- IntentParameter
-  init(title:description:default:requestValueDialog:requestDisambiguationDialog:inputConnectionBehavior:supportedValues:resolvers:) 

Initializer

# init(title:description:default:requestValueDialog:requestDisambiguationDialog:inputConnectionBehavior:supportedValues:resolvers:)

Creates an app intent parameter that can convert the selected value.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0+watchOS 9.0–11.0Deprecated

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

## See Also

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType])

Creates an app intent parameter.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType])

Creates an app intent parameter.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType], optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType], optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType], resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

