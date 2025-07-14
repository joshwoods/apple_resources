

- App Intents
- Parameter resolution
- IntentParameter
-  App entities 

API Collection

# App entities

Configure the details for parameter variables that contain custom app entities.

## Topics

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: [IntentWidgetFamily : IntentCollectionSize], inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter for an array with a specified size per widget family.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: IntentCollectionSize, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter for an array with a specified size.

convenience init&lt;Query>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: [IntentWidgetFamily : IntentCollectionSize], inputConnectionBehavior: InputConnectionBehavior, query: Query)

Creates an app intent parameter for an array with a specified size per widget family.

convenience init&lt;Query>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: IntentCollectionSize, inputConnectionBehavior: InputConnectionBehavior, query: Query)

Creates an app intent parameter for an array with a specified size.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: IntentCollectionSize, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter for an array with a specified size.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: [IntentWidgetFamily : IntentCollectionSize], inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter for an array with a specified size per widget family.

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: IntentCollectionSize, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter for an array with a specified size.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, requestValueDialog: IntentDialog?, requestDisambiguationDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

## See Also

### Creating an intent parameter for custom types

App enums

Configure the details for parameter variables that contain custom app enums.

