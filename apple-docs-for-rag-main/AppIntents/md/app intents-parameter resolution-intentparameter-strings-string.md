

- App Intents
- Parameter resolution
- IntentParameter
-  Strings 

API Collection

# Strings

Configure the details for parameter variables that contain strings or attributed strings.

## Topics

### Creating an intent parameter for a string

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, inputOptions: String.IntentInputOptions?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, inputOptions: String.IntentInputOptions?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, inputOptions: String.IntentInputOptions?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, inputOptions: String.IntentInputOptions?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

### Creating an intent parameter for an attributed string

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

### Accessing the input options

var inputOptions: String.IntentInputOptions?

## See Also

### Creating an intent parameter for primitive types

Integers

Configure the details for parameter variables that contain integers.

Doubles

Configure the details for parameter variables that contain floating-point values.

Booleans

Configure the details for parameter variables that contain Boolean values.

URLs

Configure the details for parameter variables that contain URLs.

