

- MusicKit
- MusicPersonalRecommendationsRequest
-  init(refreshing:) 

Initializer

# init(refreshing:)

Creates a request to fetch default personal recommendations for the user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(refreshing recommendations: S) where S : Sequence, S.Element == MusicPersonalRecommendation
```

