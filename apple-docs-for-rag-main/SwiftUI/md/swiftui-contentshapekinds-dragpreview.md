

- SwiftUI
- ContentShapeKinds
-  dragPreview 

Type Property

# dragPreview

The kind for drag and drop previews.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static let dragPreview: ContentShapeKinds
```

## Mentioned in 

Making a view into a drag source

## Discussion

When using this kind, only the preview shape is affected. To control the shape used to hit-test and start the drag preview, use the `interaction` kind.

## See Also

### Getting shape kinds

static let interaction: ContentShapeKinds

The kind for hit-testing and accessibility.

static let contextMenuPreview: ContentShapeKinds

The kind for context menu previews.

static let focusEffect: ContentShapeKinds

The kind for the focus effect.

static let hoverEffect: ContentShapeKinds

The kind for hover effects.

static let accessibility: ContentShapeKinds

The kind for accessibility visuals and sorting.

