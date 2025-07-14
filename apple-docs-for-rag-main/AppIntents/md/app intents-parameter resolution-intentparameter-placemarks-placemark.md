

- App Intents
- Parameter resolution
- IntentParameter
-  Placemarks 

API Collection

# Placemarks

Configure the details for parameter variables that contain a geographic location.

## Topics

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

### Accessing the display style

var displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle?

enum PlacemarkDisplayStyle

Describes a location’s display style in Shortcuts and Siri Suggestions.

## See Also

### Creating an intent parameter for common framework types

Dates

Configure the details for parameter variables that contain date values.

Date components

Configure the details for parameter variables that contain date components.

Files

Configure the details for parameter variables that contain files.

Currencies

Configure the details for parameter variables that contain currency values.

Payments

Configure the details for parameter variables that contain payment-related values.

People

Configure the details for parameter variables that contain references to people.

Measurements

Configure the details for parameter variables that contain, among others, temperature, mass, speed, energy, duration, length, and volume values.

