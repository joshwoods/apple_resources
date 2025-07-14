

- Assignables
- AssignableDocument
-  pageThumbnails(visibleParts:) 

Instance Method

# pageThumbnails(visibleParts:)

Exports thumbnails of each page such that the thumbnails contain the indicated layers.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func pageThumbnails(visibleParts: [MergeablePartsContainerPartID]) async -> [Self.Page.ID : Self.Page.Thumbnail]
```

Available when `Page.ID` is `Self.Page.Document.Page.ID`.

## Parameters 

`visibleParts`  

The lDs of layers that should be included in the thumbnail.

