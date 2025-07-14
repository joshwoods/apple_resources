

- App Intents
-  IsBetweenComparator 

Class

# IsBetweenComparator

This comparator is only supported for `Date` types in Shortcuts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final class IsBetweenComparator where Property : EntityProperty, PropertyType : _IntentValue, PropertyType : Sendable, InputType : Comparable, InputType == PropertyType.UnwrappedType
```

## Topics

### Initializers

init(mappingTransform: (InputType, InputType) -> ComparatorMappingType)

Declares support for `Between` comparisons between a property and user-supplied values.

init&lt;Spec>(withResolvers: () -> Spec, mappingTransform: (InputType, InputType) -> ComparatorMappingType)

Declares support for `Between` comparisons between a property and user-supplied values.

## Relationships

### Inherits From

- EntityQueryComparator

## See Also

### Equatable comparisons

class EqualToComparator

An object that determines whether the value of an equatable property is equal to the specified value.

class NotEqualToComparator

An object that determines whether the value of an equatable property is not equal to the specified value.

class GreaterThanComparator

An object that determines whether the value of a comparable property is greater than the specified value.

class GreaterThanOrEqualToComparator

An object that determines whether the value of a comparable property is greater than or equal to the specified value.

class LessThanComparator

An object that determines whether the value of a comparable property is less than the specified value.

class LessThanOrEqualToComparator

An object that determines whether the value of a comparable property is less than or equal to the specified value.

