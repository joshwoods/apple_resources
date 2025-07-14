

- MusicKit
- MusicCatalogChartsRequest
-  init(genre:kinds:types:) 

Initializer

# init(genre:kinds:types:)

Creates a catalog charts request for a specified genre and list of types to include in the catalog charts response.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    genre: Genre? = nil,
    kinds: [MusicCatalogChartKind] = [.mostPlayed],
    types: [any MusicCatalogChartRequestable.Type]
)
```

