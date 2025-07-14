

- App Intents
- IntentParameter
-  init(title:description:defaultValue:defaultUnit:defaultUnitAdjustForLocale:supportsNegativeNumbers:requestValueDialog:inputConnectionBehavior:) 

Initializer

# init(title:description:defaultValue:defaultUnit:defaultUnitAdjustForLocale:supportsNegativeNumbers:requestValueDialog:inputConnectionBehavior:)

Creates an app intent parameter with a default unit for the measurement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    defaultValue: Double? = nil,
    defaultUnit: IntentParameter.ElectricResistance? = nil,
    defaultUnitAdjustForLocale: Bool = false,
    supportsNegativeNumbers: Bool = true,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`defaultUnit`  

The default unit that should be selected when this parameter is initially created.

`defaultUnitAdjustForLocale`  

Whether or not the default unit should adjust to match someone’s locale. Default value is `false`.

`supportsNegativeNumbers`  

Whether or not this parameter supports negative number inputs. Default value is `true`.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

## See Also

### Creating an intent parameter

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, defaultValue: Double?, defaultUnit: IntentParameter&lt;Value>.ElectricResistance?, defaultUnitAdjustForLocale: Bool, supportsNegativeNumbers: Bool, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter with a default unit for the measurement.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, defaultValue: Double?, unit: IntentParameter&lt;Value>.ElectricResistance, unitAdjustForLocale: Bool, supportsNegativeNumbers: Bool, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter that specifies the unit for the measurement.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, defaultValue: Double?, unit: IntentParameter&lt;Value>.ElectricResistance, unitAdjustForLocale: Bool, supportsNegativeNumbers: Bool, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that specifies the unit for the measurement.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

