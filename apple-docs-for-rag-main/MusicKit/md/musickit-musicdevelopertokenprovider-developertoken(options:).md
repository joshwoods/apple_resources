

- MusicKit
- MusicDeveloperTokenProvider
-  developerToken(options:) 

Instance Method

# developerToken(options:)

Fetches and returns a developer token for Apple Music API.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func developerToken(options: MusicTokenRequestOptions) async throws -> String
```

**Required**

## Discussion

If you opt to create a custom implementation of the MusicDeveloperTokenProvider protocol, make sure to discard any cached developer token if the `options` parameter contains ignoreCache.

You can add the newly generated token to an in-memory or persistent cache for faster access upon subsequent requests for this token.

