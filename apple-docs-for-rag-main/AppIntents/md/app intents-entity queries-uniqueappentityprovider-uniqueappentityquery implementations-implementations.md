

- App Intents
- Entity queries
- UniqueAppEntityProvider
-  UniqueAppEntityQuery Implementations 

API Collection

# UniqueAppEntityQuery Implementations

## Topics

### Instance Methods

func allEntities() async throws -> [Self.Unique]

func entities(for: [Self.Unique.ID]) async throws -> [Self.Unique]

func suggestedEntities() async throws -> [Self.Unique]

