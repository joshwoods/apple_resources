

- App Intents
- Parameter resolution
- IntentParameter
-  Files 

API Collection

# Files

Configure the details for parameter variables that contain files.

## Topics

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, supportedTypeIdentifiers: [String], requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

Deprecated

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, supportedTypeIdentifiers: [String], requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

Deprecated

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, supportedTypeIdentifiers: [String], requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

Deprecated

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, supportedTypeIdentifiers: [String], requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

Deprecated

## See Also

### Creating an intent parameter for common framework types

Dates

Configure the details for parameter variables that contain date values.

Date components

Configure the details for parameter variables that contain date components.

Currencies

Configure the details for parameter variables that contain currency values.

Payments

Configure the details for parameter variables that contain payment-related values.

People

Configure the details for parameter variables that contain references to people.

Placemarks

Configure the details for parameter variables that contain a geographic location.

Measurements

Configure the details for parameter variables that contain, among others, temperature, mass, speed, energy, duration, length, and volume values.

