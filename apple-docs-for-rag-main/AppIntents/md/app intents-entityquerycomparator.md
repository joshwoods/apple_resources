

- App Intents
-  EntityQueryComparator 

Class

# EntityQueryComparator

The base class for all concrete entity query comparators.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class EntityQueryComparator where Property : EntityProperty, PropertyType : _IntentValue, PropertyType : Sendable, InputType : _IntentValue
```

## Overview

An entity query comparator specifies a particular query comparison that can be made against a EntityQueryProperty. For each query property comparator, `mappingTransform` maps the user-supplied `Value` at runtime into a `ComparatorMappingType` type of your choice.

The following example illustrates the declaration of a EntityQueryProperty on a fictional `IntentPersonEntity` that allows finding entities by strict equality or prefix on the entity `firstName` property by defining its supported `EntityQueryComparator`s:

```
Property(\.$firstName) {
   EqualToComparator { value in
        // This is called at runtime with `value` being the user-supplied value.
        // For example, value would be: "John" when the user says:
        // "Hey Siri, find persons named John", given the appropriate mapping
        // in the application's Siri metadata.

        // This closure returns an object of type `ComparatorMappingType`. In the context of
        // a `EntityQuery`, every `EntityQueryComparator` must return the same output type,
        // which is the Query's `ComparatorMappingType`.
        return "firstName must be equal to \{value}"
   }
   HasPrefixComparator { "firstName must start with \{$0}" }
}
```

## Resolvers

Additionally, you can supply a set of Resolvers to fine-tune how the system will transform a user’s supplied value into into the target `Value` type.

## Relationships

### Inherited By

- ContainsComparator
- EqualToComparator
- GreaterThanComparator
- GreaterThanOrEqualToComparator
- HasPrefixComparator
- HasSuffixComparator
- IsBetweenComparator
- LessThanComparator
- LessThanOrEqualToComparator
- NotEqualToComparator

## See Also

### Building query comparators

static func buildBlock(AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>...) -> [AnyEntityQueryComparator&lt;Entity, Subject, Property, PropertyType, ComparatorMappingType>]

struct AnyEntityQueryComparator

A type that erases the type information of the underlying query comparator.

