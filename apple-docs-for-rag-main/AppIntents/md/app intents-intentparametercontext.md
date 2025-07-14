

- App Intents
-  IntentParameterContext 

Structure

# IntentParameterContext

A type that provides information about an associated parameter during value resolution.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentParameterContext where Value : _IntentValue, Value : Sendable
```

## Topics

### Instance Properties

var controlStyle: IntentParameter&lt;Value>.IntControlStyle?

var controlStyle: IntentParameter&lt;Value>.DoubleControlStyle?

var currencyCodes: [String]?

var dateKind: IntentParameter&lt;Value>.DateKind?

var dateKind: IntentParameter&lt;Value>.DateKind?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitFuelEfficiency>>.FuelEfficiency?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitLength>>.Length?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitAcceleration>>.Acceleration?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitElectricResistance>>.ElectricResistance?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitDispersion>>.Dispersion?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitVolume>>.Volume?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitMass>>.Mass?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitConcentrationMass>>.ConcentrationMass?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitElectricPotentialDifference>>.ElectricPotentialDifference?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitEnergy>>.Energy?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitFrequency>>.Frequency?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitElectricCharge>>.ElectricCharge?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitTemperature>>.Temperature?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitAngle>>.Angle?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitArea>>.Area?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitDuration>>.Duration?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitIlluminance>>.Illuminance?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitInformationStorage>>.InformationStorage?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitPower>>.Power?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitPressure>>.Pressure?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitSpeed>>.Speed?

var defaultUnit: IntentParameter&lt;Measurement&lt;UnitElectricCurrent>>.ElectricCurrent?

var displayName: Bool.IntentDisplayName?

var displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle?

var inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?

var inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Double>?

var inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Int>?

var isOptional: Bool

var parameterMode: IntentPerson.ParameterMode?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var supportsNegativeNumbers: Bool?

var title: LocalizedStringResource

var unit: IntentParameter&lt;Measurement&lt;UnitPower>>.Power?

var unit: IntentParameter&lt;Measurement&lt;UnitElectricPotentialDifference>>.ElectricPotentialDifference?

var unit: IntentParameter&lt;Measurement&lt;UnitMass>>.Mass?

var unit: IntentParameter&lt;Measurement&lt;UnitElectricCurrent>>.ElectricCurrent?

var unit: IntentParameter&lt;Measurement&lt;UnitSpeed>>.Speed?

var unit: IntentParameter&lt;Measurement&lt;UnitElectricResistance>>.ElectricResistance?

var unit: IntentParameter&lt;Measurement&lt;UnitTemperature>>.Temperature?

var unit: IntentParameter&lt;Measurement&lt;UnitPressure>>.Pressure?

var unit: IntentParameter&lt;Measurement&lt;UnitDispersion>>.Dispersion?

var unit: IntentParameter&lt;Measurement&lt;UnitArea>>.Area?

var unit: IntentParameter&lt;Measurement&lt;UnitLength>>.Length?

var unit: IntentParameter&lt;Measurement&lt;UnitElectricCharge>>.ElectricCharge?

var unit: IntentParameter&lt;Measurement&lt;UnitVolume>>.Volume?

var unit: IntentParameter&lt;Measurement&lt;UnitInformationStorage>>.InformationStorage?

var unit: IntentParameter&lt;Measurement&lt;UnitFrequency>>.Frequency?

var unit: IntentParameter&lt;Measurement&lt;UnitAngle>>.Angle?

var unit: IntentParameter&lt;Measurement&lt;UnitIlluminance>>.Illuminance?

var unit: IntentParameter&lt;Measurement&lt;UnitEnergy>>.Energy?

var unit: IntentParameter&lt;Measurement&lt;UnitFuelEfficiency>>.FuelEfficiency?

var unit: IntentParameter&lt;Measurement&lt;UnitConcentrationMass>>.ConcentrationMass?

var unit: IntentParameter&lt;Measurement&lt;UnitAcceleration>>.Acceleration?

var unit: IntentParameter&lt;Measurement&lt;UnitDuration>>.Duration?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

var unitAdjustForLocale: Bool?

### Instance Methods

func needsDisambiguationError(among: [Value.ValueType], dialog: IntentDialog?) -> AppIntentError

Returns a `restartPerform` error with context for the user to disambiguate amongst an array of values from for this parameter and re-perform the intent with the new value.

func needsValueError(IntentDialog?) -> AppIntentError

Returns a `restartPerform` error with context to request a value from the user for this parameter and re-perform the intent with the new value.

func requestConfirmation(for: Value.ValueType, dialog: IntentDialog?) async throws -> Bool

Use `requestConfirmation` when you need to the ask user to confirm the parameter value.

func requestConfirmation&lt;ViewType>(for: Value.ValueType, dialog: IntentDialog?, view: ViewType) async throws -> Bool

Use `requestConfirmation` when you need to the ask user to confirm the parameter value.

func requestConfirmation&lt;ViewType>(for: Value.ValueType, dialog: IntentDialog?, view: () -> ViewType) async throws -> Bool

Use `requestConfirmation` when you need to the ask user to confirm the parameter value.

func requestDisambiguation(among: [Value.ValueType], dialog: IntentDialog?) async throws -> Value.ValueType

Request that the user disambiguate amongst an array of values for this parameter.

func requestValue(IntentDialog?) async throws -> Value.ValueType

Request a value from the user for this parameter.

## Relationships

### Conforms To

- AnyIntentValue
- Sendable

## See Also

### Intent parameters

class IntentParameter

A property wrapper that indicates the associated property is an input argument of the app intent.

class IntentParameterDependency

A property wrapper that represents an app intent dependency you use to provide dynamic options.

enum InputConnectionBehavior

Describes the input behaviors for connecting a parameter to the output of the previous App Intent.

