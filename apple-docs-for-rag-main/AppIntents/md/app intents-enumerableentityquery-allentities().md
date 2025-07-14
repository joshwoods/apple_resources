

- App Intents
- EnumerableEntityQuery
-  allEntities() 

Instance Method

# allEntities()

Returns all available results.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func allEntities() async throws -> Self.Result
```

**Required** Default implementation provided.

## Default Implementations

### EnumerableEntityQuery Implementations

func allEntities() async throws -> [Self.Unique]

