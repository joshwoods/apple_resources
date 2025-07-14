

- App Intents
-  HasSuffixComparator 

Class

# HasSuffixComparator

An object that determines whether the value of a string property has the specified suffix.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final class HasSuffixComparator where Property : EntityProperty, PropertyType : _IntentValue, PropertyType : Sendable, InputType : _IntentValue
```

## Topics

### Initializers

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `hasSuffix` operator between a `String` property and user-supplied values.

init(mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `hasSuffix` operator between a `String?` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `hasSuffix` operator between a `String?` property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType) -> ComparatorMappingType)

Declares support for the `hasSuffix` operator between a `String` property and user-supplied values.

## Relationships

### Inherits From

- EntityQueryComparator

## See Also

### String comparisons

class HasPrefixComparator

An object that determines whether the value of a string property has the specified prefix.

enum StringComparisonOperator

