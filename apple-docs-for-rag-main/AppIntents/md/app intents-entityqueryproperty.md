

- App Intents
-  EntityQueryProperty 

Class

# EntityQueryProperty

An object that provides the supported comparators you use to describe the different ways users can query against a property of an app entity.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final class EntityQueryProperty where Entity : AppEntity, Subject : AppEntity, Property : EntityProperty, PropertyType : _IntentValue, PropertyType : Sendable
```

## Overview

Entity query properties are defined by by providing a `KeyPath` to an `AppEntity` property in your data model that this property applies to and then specify the set of supported EntityQueryComparators for this property.

`EntityQueryProperty` allows you to define `EntityQueryComparator`s beyond strict equality. The set of comparators available depends on the underlying property type. For example, an `Equatable` property type will allow for `EqualToComparator` and `NotEqualToComparator` comparators while a `Comparable` property type will add support for `GreaterThanComparator`, `GreaterThanOrEqualToComparator`, `LessThanComparator`, and `LessThanOrEqualToComparator` comparators. See `Comparator` for more details on available comparators.

An `EntityQueryProperty` doesn’t necessarily need to apply to a property of its parent Query `Entity`.

Consider the scenario where you have an application containing Photo and Album entities, and you want to support querying photos by the name of their containing album. Within a EntityPropertyQuery in which `Entity` is Photo, you can define a `EntityQueryProperty` mapping to a name property of the Album entity, as long as you supply a closure for `entityProvider` that contains the logic to get from a Photo entity to an Album entity.

See `EntityQueryProperty/init(title:entityProvider:keyPath:)` for details.

## Topics

### Creating queryable properties

typealias QueryComparators

A type alias for the type that represents a collection of query comparators.

enum EntityQueryComparatorsBuilder

A result builder that allows you to declaratively describe the comparators for a queryable property.

### Initializers

convenience init(KeyPath&lt;Subject, Property>, comparators: () -> EntityQueryProperty&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>.QueryComparators)

Initializes a EntityQueryProperty that applies to entity property at the provided keyPath.

init(KeyPath&lt;Subject, Property>, entityProvider: (Entity) -> Subject, comparators: () -> EntityQueryProperty&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>.QueryComparators)

Initializes a EntityQueryProperty that applies to entity property at the provided keyPath.

## Relationships

### Inherits From

- EntityQueryPropertyDeclaration

## See Also

### Property-matched queries

protocol EntityPropertyQuery

An interface for locating entities by matching values against one or more of their properties.

struct EntityQueryProperties

A type that provides the properties to include in a property-matched query.

Property comparators

Specify the type of comparison to perform during a property-matched query.

struct EntityQuerySortingOptions

The potential properties you can use to sort the results of a query.

struct EntityQuerySortableByProperty

Details about a specific property you use to sort the query results.

struct EntityQuerySort

The properties to use to sort the results when the query runs.

