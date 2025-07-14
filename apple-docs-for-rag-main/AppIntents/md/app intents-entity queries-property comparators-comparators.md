

- App Intents
- Entity queries
-  Property comparators 

API Collection

# Property comparators

Specify the type of comparison to perform during a property-matched query.

## Topics

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

class IsBetweenComparator

This comparator is only supported for `Date` types in Shortcuts.

### String comparisons

class HasPrefixComparator

An object that determines whether the value of a string property has the specified prefix.

class HasSuffixComparator

An object that determines whether the value of a string property has the specified suffix.

enum StringComparisonOperator

### Containment comparisons

class ContainsComparator

An object that determines whether the value of sequence property contains the specified value.

## See Also

### Property-matched queries

protocol EntityPropertyQuery

An interface for locating entities by matching values against one or more of their properties.

struct EntityQueryProperties

A type that provides the properties to include in a property-matched query.

class EntityQueryProperty

An object that provides the supported comparators you use to describe the different ways users can query against a property of an app entity.

struct EntityQuerySortingOptions

The potential properties you can use to sort the results of a query.

struct EntityQuerySortableByProperty

Details about a specific property you use to sort the query results.

struct EntityQuerySort

The properties to use to sort the results when the query runs.

