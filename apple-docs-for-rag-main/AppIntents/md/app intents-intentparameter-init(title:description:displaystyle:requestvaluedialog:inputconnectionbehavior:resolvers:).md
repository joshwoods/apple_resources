

- App Intents
- IntentParameter
-  init(title:description:displayStyle:requestValueDialog:inputConnectionBehavior:resolvers:) 

Initializer

# init(title:description:displayStyle:requestValueDialog:inputConnectionBehavior:resolvers:)

Creates an app intent parameter that can convert the selected value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    displayStyle: IntentParameter.PlacemarkDisplayStyle = .name,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default,
    @ResolverSpecificationBuilder resolvers: @escaping () -> Spec
) where Spec : ResolverSpecification
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `CLPlacemark`.

## Parameters 

`title`  

A word or short phrase summarizing this parameter.

`description`  

Additional details about this parameter.

`displayStyle`  

The component of a selected location to display, such as a city or street address.

`requestValueDialog`  

A prompt that asks a person to provide the parameter value.

`inputConnectionBehavior`  

An enum that indicates how this parameter receives the output from a preceding app intent.

`resolvers`  

An object that converts a value of another type to this parameter’s type.

## See Also

### Creating an intent parameter

convenience init(title: LocalizedStringResource, description: LocalizedStringResource?, displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior)

Creates an app intent parameter.

convenience init&lt;OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider)

Creates an app intent parameter with a list of selectable options.

convenience init&lt;Spec, OptionsProvider>(title: LocalizedStringResource, description: LocalizedStringResource?, displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle, requestValueDialog: IntentDialog?, inputConnectionBehavior: InputConnectionBehavior, optionsProvider: OptionsProvider, resolvers: () -> Spec)

Creates an app intent parameter with a list of selectable options that can convert the selected value.

