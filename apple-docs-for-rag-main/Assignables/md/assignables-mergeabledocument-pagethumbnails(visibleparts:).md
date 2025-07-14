

- Assignables
- MergeableDocument
-  pageThumbnails(visibleParts:) 

Instance Method

# pageThumbnails(visibleParts:)

Exports thumbnails of each page such that the thumbnails contain the indicated layers.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func pageThumbnails(visibleParts: [Self.PartID]) async -> [Self.Page.ID : Self.Page.Thumbnail]
```

**Required** Default implementation provided.

## Parameters 

`visibleParts`  

The lDs of layers that should be included in the thumbnail.

## Default Implementations

### MergeableDocument Implementations

func pageThumbnails(visibleParts: [MergeablePartsContainerPartID]) async -> [Self.Page.ID : Self.Page.Thumbnail]

Exports thumbnails of each page such that the thumbnails contain the indicated layers.

