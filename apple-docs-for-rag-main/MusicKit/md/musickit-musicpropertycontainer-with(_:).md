

- MusicKit
- MusicPropertyContainer
-  with(\_:) 

Instance Method

# with(\_:)

Loads a new instance of the music item that includes the specified properties.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func with(_ properties: [PartialMusicAsyncProperty]) async throws -> Self
```

**Required** Default implementation provided.

## Discussion

This asynchronous method fetches a more complete representation of the receiver from Apple Music API over the network.

## Default Implementations

### MusicPropertyContainer Implementations

func with(PartialMusicAsyncProperty&lt;Self>...) async throws -> Self

Loads a new instance of the music item that includes the specified properties.

