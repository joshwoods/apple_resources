

- App Intents
-  EntityQueryPropertiesBuilder 

Enumeration

# EntityQueryPropertiesBuilder

A result builder that allows you to declaratively describe the properties to include in a property-matched query.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum EntityQueryPropertiesBuilder where Entity : AppEntity
```

## Topics

### Building queryable properties

static func buildBlock(EntityQueryPropertyDeclaration&lt;Entity, ComparatorMappingType>...) -> [EntityQueryPropertyDeclaration&lt;Entity, ComparatorMappingType>]

class EntityQueryPropertyDeclaration

An object that identifies a specific entity property and the query comparators it supports.

### Type Methods

static func buildExpression(EntityQueryPropertyDeclaration&lt;Entity, ComparatorMappingType>) -> EntityQueryPropertyDeclaration&lt;Entity, ComparatorMappingType>

