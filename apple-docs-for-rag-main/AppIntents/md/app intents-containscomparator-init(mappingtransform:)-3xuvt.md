

- App Intents
- ContainsComparator
-  init(mappingTransform:) 

Initializer

# init(mappingTransform:)

Declares support for the `contains` operator between a `String` property and user-supplied values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(mappingTransform: @escaping (InputType) -> ComparatorMappingType) where Property : EntityProperty, PropertyType == String, InputType == String
```

## Parameters 

`mappingTransform`  

Closure that transforms the user-supplied value into the `ComparatorMappingType` output type.

