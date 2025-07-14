

- App Intents
- IntentParameter
-  init(title:description:default:size:inputConnectionBehavior:query:) 

Initializer

# init(title:description:default:size:inputConnectionBehavior:query:)

Creates an app intent parameter for an array with a specified size.

iOS 17.0–18.0DeprecatediPadOS 17.0–18.0DeprecatedMac Catalyst 17.0–18.0DeprecatedmacOS 14.0–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0+watchOS 10.0–11.0Deprecated

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    default defaultValue: Value.UnwrappedType? = nil,
    size: IntentCollectionSize,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    query: Query
) where Query : EntityQuery, Value.ValueType == Query.Entity
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, `Value.UnwrappedType` conforms to `Collection`, and `Value.ValueType` conforms to `AppEntity`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`defaultValue`  

The default value for this parameter. People can specify a different value.

`size`  

The size of the array you specify to limit the amount of values.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`query`  

A query that Siri and the Shortcuts app can use to retrieve instances of your entity.

## See Also

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: [IntentWidgetFamily : IntentCollectionSize], inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter for an array with a specified size per widget family.

convenience init&lt;Spec>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: IntentCollectionSize, inputConnectionBehavior: InputConnectionBehavior, resolvers: () -> Spec)

Creates an app intent parameter for an array with a specified size.

convenience init&lt;Query>(title: LocalizedStringResource, description: LocalizedStringResource?, default: Value.UnwrappedType?, size: [IntentWidgetFamily : IntentCollectionSize], inputConnectionBehavior: InputConnectionBehavior, query: Query)

Creates an app intent parameter for an array with a specified size per widget family.

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

