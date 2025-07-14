

- Core Spotlight
- CSSearchableIndex
-  deleteAppEntities(identifiedBy:ofType:) 

Instance Method

# deleteAppEntities(identifiedBy:ofType:)

Deletes specific app entities from the system’s index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func deleteAppEntities(
    identifiedBy identifiers: [Entity.ID],
    ofType type: Entity.Type
) async throws where Entity : IndexedEntity
```

