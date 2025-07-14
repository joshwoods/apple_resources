

- App Intents
-  ContainsComparator 

Class

# ContainsComparator

An object that determines whether the value of sequence property contains the specified value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final class ContainsComparator where Property : EntityProperty, PropertyType : _IntentValue, PropertyType : Sendable, InputType : _IntentValue
```

## Topics

### Initializers

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `String` property and user-supplied values.

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between an optional `Array` property and user-supplied values.

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `AttributedString?` property and user-supplied values.

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `String?` property and user-supplied values.

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between an `Array` property and user-supplied values.

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `AttributedString` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `String` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between an `Array` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `String?` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between an optional `Array` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `AttributedString` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `contains` operator between a `AttributedString?` property and user-supplied values.

## Relationships

### Inherits From

- EntityQueryComparator

