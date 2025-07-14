

- App Intents
- IntentParameter
-  init(title:description:default:currencyCodes:inclusiveRange:requestValueDialog:inputConnectionBehavior:) 

Initializer

# init(title:description:default:currencyCodes:inclusiveRange:requestValueDialog:inputConnectionBehavior:)

Creates an app intent parameter.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    currencyCodes: [String] = [],
    inclusiveRange: IntentParameter.InclusiveRange? = nil,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `IntentCurrencyAmount`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`currencyCodes`  

A list of selectable currency symbols for this parameter. Use ISO 4217 currency codes. The default value is an empty array which offers all currency codes to a person.

`inclusiveRange`  

The allowed minimum and maximum values for this parameter.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

