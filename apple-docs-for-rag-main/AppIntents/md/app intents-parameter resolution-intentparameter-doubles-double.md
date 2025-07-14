

- App Intents
- Parameter resolution
- IntentParameter
-  Doubles 

API Collection

# Doubles

Configure the details for parameter variables that contain floating-point values.

## Topics

### Creating an intent parameter

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, controlStyle: IntentParameter&lt;Value>.DoubleControlStyle, inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Value.ValueType>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, controlStyle: IntentParameter&lt;Value>.DoubleControlStyle, inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Value.ValueType>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, controlStyle: IntentParameter&lt;Value>.DoubleControlStyle, inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Value.ValueType>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, controlStyle: IntentParameter&lt;Value>.DoubleControlStyle, inclusiveRange: IntentParameter&lt;Value>.InclusiveRange&lt;Value.ValueType>?, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

typealias InclusiveRange

### Accessing the control style

var controlStyle: IntentParameter&lt;Value>.DoubleControlStyle?

enum DoubleControlStyle

An enum that describes the control style of a Double parameter.

## See Also

### Creating an intent parameter for primitive types

Integers

Configure the details for parameter variables that contain integers.

Booleans

Configure the details for parameter variables that contain Boolean values.

Strings

Configure the details for parameter variables that contain strings or attributed strings.

URLs

Configure the details for parameter variables that contain URLs.

