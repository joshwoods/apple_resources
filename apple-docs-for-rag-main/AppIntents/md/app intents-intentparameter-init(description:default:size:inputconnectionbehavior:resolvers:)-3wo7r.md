

- App Intents
- IntentParameter
-  init(description:default:size:inputConnectionBehavior:resolvers:) 

Initializer

# init(description:default:size:inputConnectionBehavior:resolvers:)

Creates an app intent parameter for an array with a specified size per widget family.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    size: [IntentWidgetFamily : IntentCollectionSize],
    inputConnectionBehavior: InputConnectionBehavior = .default,
    @ResolverSpecificationBuilder resolvers: @escaping () -> Spec
) where Spec : ResolverSpecification
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, `Value.UnwrappedType` conforms to `Collection`, and `Value.ValueType` conforms to `AppEntity`.

## Parameters 

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`size`  

The size of the array for a widget family. Use this to limit the amount of values.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`resolvers`  

An object that converts a value of another type to this parameter’s type.

