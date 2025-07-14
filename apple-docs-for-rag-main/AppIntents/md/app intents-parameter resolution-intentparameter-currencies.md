

- App Intents
- Parameter resolution
- IntentParameter
-  Currencies 

API Collection

# Currencies

Configure the details for parameter variables that contain currency values.

## Topics

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, currencyCodes: [String], inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, currencyCodes: [String], inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, currencyCodes: [String], inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, currencyCodes: [String], inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

### Accessing the configuration

var currencyCodes: [String]?

var inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Decimal>?

typealias InclusiveRange

## See Also

### Creating an intent parameter for common framework types

Dates

Configure the details for parameter variables that contain date values.

Date components

Configure the details for parameter variables that contain date components.

Files

Configure the details for parameter variables that contain files.

Payments

Configure the details for parameter variables that contain payment-related values.

People

Configure the details for parameter variables that contain references to people.

Placemarks

Configure the details for parameter variables that contain a geographic location.

Measurements

Configure the details for parameter variables that contain, among others, temperature, mass, speed, energy, duration, length, and volume values.

