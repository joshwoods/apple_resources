

- App Intents
- NotEqualToComparator
-  init(mappingTransform:) 

Initializer

# init(mappingTransform:)

Declares support for `Equatable` `!=` comparisons between a property and user-supplied values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(mappingTransform: @escaping (PropertyType) -> ComparatorMappingType)
```

## Parameters 

`mappingTransform`  

Closure that transforms the user-supplied value into the `ComparatorMappingType` output type.

## See Also

### Creating a comparator

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (PropertyType) -> ComparatorMappingType)

Declares support for `Equatable` `!=` comparisons between a property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (PropertyType) -> ComparatorMappingType)

Declares support for `Equatable` `!=` comparisons between a property and user-supplied values.

