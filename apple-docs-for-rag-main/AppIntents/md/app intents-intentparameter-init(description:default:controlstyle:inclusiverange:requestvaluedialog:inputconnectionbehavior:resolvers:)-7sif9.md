

- App Intents
- IntentParameter
-  init(description:default:controlStyle:inclusiveRange:requestValueDialog:inputConnectionBehavior:resolvers:) 

Initializer

# init(description:default:controlStyle:inclusiveRange:requestValueDialog:inputConnectionBehavior:resolvers:)

Creates an app intent parameter that can convert the selected value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    controlStyle: IntentParameter.DoubleControlStyle = .stepper,
    inclusiveRange: IntentParameter.InclusiveRange? = nil,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    @ResolverSpecificationBuilder resolvers: @escaping () -> Spec
) where Spec : ResolverSpecification
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Double`.

## Parameters 

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

