

- App Intents
- EntityIdentifier
-  init(for:) 

Initializer

# init(for:)

Creates an identifier for the specified entity

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(for entity: Entity) where Entity : AppEntity
```

## See Also

### Creating an entity identifier

init&lt;Entity>(for: Entity.Type, identifier: Entity.ID)

Creates an `EntityIdentifier` representing an instance of the specified entity type backed by the specified identifier value.

