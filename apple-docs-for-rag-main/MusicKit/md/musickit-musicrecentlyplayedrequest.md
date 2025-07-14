

- MusicKit
-  MusicRecentlyPlayedRequest 

Structure

# MusicRecentlyPlayedRequest

A request that your app uses to fetch items the user has recently played.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicRecentlyPlayedRequest where MusicItemType : MusicRecentlyPlayedRequestable, MusicItemType : Decodable
```

## Topics

### Initializers

init()

Creates a request for items the user has recently played.

### Instance Properties

var limit: Int?

A limit for the number of items to return in the response that contains items the user has recently played.

var offset: Int?

An offet for the request.

### Instance Methods

func response() async throws -> MusicRecentlyPlayedResponse&lt;MusicItemType>

Fetches items the user has recently played.

