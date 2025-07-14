

- App Intents
- EntityQuery
-  suggestedEntities() 

Instance Method

# suggestedEntities()

Returns the initial results shown when a list of options backed by this query is presented.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func suggestedEntities() async throws -> Self.Result
```

**Required** Default implementations provided.

## Mentioned in 

Integrating custom data types into your intents

## Default Implementations

### EntityQuery Implementations

func suggestedEntities() async throws -> Self.Result

Returns the initial results shown when a list of options backed by this query is presented.

func suggestedEntities() async throws -> Self.Result

Returns the initial results shown when a list of options backed by this query is presented.

func suggestedEntities() async throws -> [Self.Unique]

