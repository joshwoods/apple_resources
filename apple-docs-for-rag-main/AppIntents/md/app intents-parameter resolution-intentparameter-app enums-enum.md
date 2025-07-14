

- App Intents
- Parameter resolution
- IntentParameter
-  App enums 

API Collection

# App enums

Configure the details for parameter variables that contain custom app enums.

## Topics

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType])

Creates an app intent parameter.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType])

Creates an app intent parameter.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType], optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType], optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType], resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, supportedValues: [Value.ValueType], resolvers: () -> Spec)

Creates an app intent parameter that can convert the selected value.

## See Also

### Creating an intent parameter for custom types

App entities

Configure the details for parameter variables that contain custom app entities.

