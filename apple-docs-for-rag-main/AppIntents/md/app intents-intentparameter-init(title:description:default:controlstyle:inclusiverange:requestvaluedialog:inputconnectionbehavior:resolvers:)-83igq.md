

- App Intents
- IntentParameter
-  init(title:description:default:controlStyle:inclusiveRange:requestValueDialog:inputConnectionBehavior:resolvers:) 

Initializer

# init(title:description:default:controlStyle:inclusiveRange:requestValueDialog:inputConnectionBehavior:resolvers:)

Creates an app intent parameter that can convert the selected value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    controlStyle: IntentParameter.IntControlStyle = .stepper,
    inclusiveRange: IntentParameter.InclusiveRange? = nil,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    @ResolverSpecificationBuilder resolvers: @escaping () -> Spec
) where Spec : ResolverSpecification
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Int`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`controlStyle`  

The type of user input control for this parameter.

`inclusiveRange`  

The allowed minimum and maximum values for this parameter.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`resolvers`  

An object that converts a value of another type to this parameter’s type.

## See Also

### Creating an intent parameter

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, controlStyle: IntentParameter&lt;Value>.IntControlStyle, inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Value.ValueType>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, controlStyle: IntentParameter&lt;Value>.IntControlStyle, inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Value.ValueType>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, controlStyle: IntentParameter&lt;Value>.IntControlStyle, inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Value.ValueType>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

typealias InclusiveRange

