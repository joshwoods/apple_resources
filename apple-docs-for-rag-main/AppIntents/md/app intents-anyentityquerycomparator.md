

- App Intents
-  AnyEntityQueryComparator 

Structure

# AnyEntityQueryComparator

A type that erases the type information of the underlying query comparator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AnyEntityQueryComparator where Property : EntityProperty, PropertyType : _IntentValue, PropertyType : Sendable
```

## See Also

### Building query comparators

static func buildBlock(AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>...) -> [AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>]

class EntityQueryComparator

The base class for all concrete entity query comparators.

