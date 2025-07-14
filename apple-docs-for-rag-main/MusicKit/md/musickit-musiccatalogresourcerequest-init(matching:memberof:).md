

- MusicKit
- MusicCatalogResourceRequest
-  init(matching:memberOf:) 

Initializer

# init(matching:memberOf:)

Creates a request to fetch items using a filter that matches any value from an array of possible values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    matching keyPath: KeyPath,
    memberOf values: [Value]
) where MusicItemType : FilterableMusicItem
```

