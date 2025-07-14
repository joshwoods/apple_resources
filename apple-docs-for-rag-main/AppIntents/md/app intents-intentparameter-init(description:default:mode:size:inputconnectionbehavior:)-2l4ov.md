

- App Intents
- IntentParameter
-  init(description:default:mode:size:inputConnectionBehavior:) 

Initializer

# init(description:default:mode:size:inputConnectionBehavior:)

Creates an app intent parameter for an array with a specified size.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    mode: IntentPerson.ParameterMode = .contact,
    size: IntentCollectionSize,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, `Value.UnwrappedType` conforms to `Collection`, and `Value.ValueType` is `IntentPerson`.

## Parameters 

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`mode`  

The user interface that appears when a person chooses a value for this parameter. Default value is `.contact`.

`size`  

The size of the array you specify to limit the amount of values.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

