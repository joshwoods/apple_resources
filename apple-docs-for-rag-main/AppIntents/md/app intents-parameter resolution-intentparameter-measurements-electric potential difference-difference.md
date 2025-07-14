

- App Intents
- Parameter resolution
- IntentParameter
- Measurements
-  Electric potential difference 

API Collection

# Electric potential difference

Configure the details for parameter variables that contain values of electric potential difference.

## Topics

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, defaultValue: Double?, defaultUnit: IntentParameter&lt;Value>.ElectricPotentialDifference?, defaultUnitAdjustForLocale: Bool, supportsNegativeNumbers: Bool, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter with a default unit for the measurement.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, defaultValue: Double?, defaultUnit: IntentParameter&lt;Value>.ElectricPotentialDifference?, defaultUnitAdjustForLocale: Bool, supportsNegativeNumbers: Bool, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter with a default unit for the measurement.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, defaultValue: Double?, unit: IntentParameter&lt;Value>.ElectricPotentialDifference, unitAdjustForLocale: Bool, supportsNegativeNumbers: Bool, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter that specifies the unit for the measurement.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, defaultValue: Double?, unit: IntentParameter&lt;Value>.ElectricPotentialDifference, unitAdjustForLocale: Bool, supportsNegativeNumbers: Bool, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that specifies the unit for the measurement.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

### Accessing unit details

var unit: IntentParameter&lt;Value>.ElectricPotentialDifference?

enum ElectricPotentialDifference

var defaultUnit: IntentParameter&lt;Value>.ElectricPotentialDifference?

var supportsNegativeNumbers: Bool?

var unitAdjustForLocale: Bool?

## See Also

### Creating an intent parameter for measurements

Acceleration

Configure the details for parameter variables that contain acceleration values.

Angles

Configure the details for parameter variables that contain angles.

Area

Configure the details for parameter variables that contain area values.

Concentration mass

Configure the details for parameter variables that contain concentration mass values.

Dispersion

Configure the details for parameter variables that contain dispersion values.

Durations

Configure the details for parameter variables that contain durations.

Electric charge

Configure the details for parameter variables that contain electric charge values.

Electric current

Configure the details for parameter variables that contain electric current values.

Electric resistance

Configure the details for parameter variables that contain electric resistance values.

Energy

Configure the details for parameter variables that contain energy values.

Frequency

Configure the details for parameter variables that contain frequency values.

Fuel efficiency

Configure the details for parameter variables that contain fuel efficiency values.

Illuminance

Configure the details for parameter variables that contain illuminance values.

Information storage

Configure the details for parameter variables that contain information storage values.

Length

Configure the details for parameter variables that contain length values.

