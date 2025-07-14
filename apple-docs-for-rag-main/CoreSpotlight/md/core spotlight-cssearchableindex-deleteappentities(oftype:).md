

- Core Spotlight
- CSSearchableIndex
-  deleteAppEntities(ofType:) 

Instance Method

# deleteAppEntities(ofType:)

Deletes all app entities of the given type from the system indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func deleteAppEntities(ofType entityType: Entity.Type) async throws where Entity : IndexedEntity
```

