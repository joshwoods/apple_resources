

- App Intents
- IntentParameter
-  init(description:defaultValue:unit:unitAdjustForLocale:supportsNegativeNumbers:requestValueDialog:inputConnectionBehavior:) 

Initializer

# init(description:defaultValue:unit:unitAdjustForLocale:supportsNegativeNumbers:requestValueDialog:inputConnectionBehavior:)

Creates an app intent parameter that specifies the unit for the measurement.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
convenience init(
    description: LocalizedStringResource? = nil,
    defaultValue: Double? = nil,
    unit: IntentParameter.Energy,
    unitAdjustForLocale: Bool = false,
    supportsNegativeNumbers: Bool = true,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Parameters 

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`unit`  

The exact unit for this parameter. People won’t be able to change this unit.

`unitAdjustForLocale`  

Whether or not the unit should adjust to match someone’s locale. Default value is `false`.

`supportsNegativeNumbers`  

Whether or not this parameter supports negative number inputs. Default value is `true`.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

