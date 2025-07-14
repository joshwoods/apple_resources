

- App Intents
-  EntityQueryComparatorsBuilder 

Enumeration

# EntityQueryComparatorsBuilder

A result builder that allows you to declaratively describe the comparators for a queryable property.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum EntityQueryComparatorsBuilder where Entity : AppEntity, Subject : AppEntity, Property : EntityProperty, PropertyType : _IntentValue, PropertyType : Sendable
```

## Topics

### Building query comparators

static func buildBlock(AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>...) -> [AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>]

struct AnyEntityQueryComparator

A type that erases the type information of the underlying query comparator.

class EntityQueryComparator

The base class for all concrete entity query comparators.

### Type Methods

static func buildExpression(EntityQueryComparator&lt;Property, PropertyType, PropertyType.UnwrappedType, ComparatorMappingType>) -> AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>

static func buildExpression(EntityQueryComparator&lt;Property, PropertyType, PropertyType, ComparatorMappingType>) -> AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>

static func buildExpression&lt;InputType>(ContainsComparator&lt;Property, PropertyType, InputType, ComparatorMappingType>) -> AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>

static func buildExpression&lt;InputType>(IsBetweenComparator&lt;Property, PropertyType, InputType, ComparatorMappingType>) -> AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>

## See Also

### Creating queryable properties

typealias QueryComparators

A type alias for the type that represents a collection of query comparators.

