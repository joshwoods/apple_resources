

- App Intents
-  EntityQuerySortingOptionsBuilder 

Enumeration

# EntityQuerySortingOptionsBuilder

A result builder that allows you to declaratively describe the sorting options for an entity query.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum EntityQuerySortingOptionsBuilder where Entity : AppEntity
```

## Topics

### Building sorting options

static func buildBlock(EntityQuerySortableByProperty&lt;Entity>...) -> [EntityQuerySortableByProperty&lt;Entity>]

### Type Methods

static func buildExpression(EntityQuerySortableByProperty&lt;Entity>) -> EntityQuerySortableByProperty&lt;Entity>

## See Also

### Creating the sorting options

init(content: () -> [EntityQuerySortableByProperty&lt;Entity>])

