

- MusicKit
- MusicCatalogResourceRequest
-  init(matching:equalTo:) 

Initializer

# init(matching:equalTo:)

Creates a request to fetch items using a filter that matches a specific value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    matching keyPath: KeyPath,
    equalTo value: Value
) where MusicItemType : FilterableMusicItem
```

