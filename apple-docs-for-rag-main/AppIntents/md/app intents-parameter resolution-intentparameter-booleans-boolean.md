

- App Intents
- Parameter resolution
- IntentParameter
-  Booleans 

API Collection

# Booleans

Configure the details for parameter variables that contain Boolean values.

## Topics

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, displayName: Bool.IntentDisplayName?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, displayName: Bool.IntentDisplayName?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

### Specifying the display name

var displayName: Bool.IntentDisplayName?

## See Also

### Creating an intent parameter for primitive types

Integers

Configure the details for parameter variables that contain integers.

Doubles

Configure the details for parameter variables that contain floating-point values.

Strings

Configure the details for parameter variables that contain strings or attributed strings.

URLs

Configure the details for parameter variables that contain URLs.

