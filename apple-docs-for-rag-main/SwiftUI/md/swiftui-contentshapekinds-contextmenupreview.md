

- SwiftUI
- ContentShapeKinds
-  contextMenuPreview 

Type Property

# contextMenuPreview

The kind for context menu previews.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 17.0+visionOS 1.0+

``` source
static let contextMenuPreview: ContentShapeKinds
```

## Discussion

When using this kind, only the preview shape will be affected. To control the shape used to hit-test and start the context menu presentation, use the `.interaction` kind.

## See Also

### Getting shape kinds

static let interaction: ContentShapeKinds

The kind for hit-testing and accessibility.

static let dragPreview: ContentShapeKinds

The kind for drag and drop previews.

static let focusEffect: ContentShapeKinds

The kind for the focus effect.

static let hoverEffect: ContentShapeKinds

The kind for hover effects.

static let accessibility: ContentShapeKinds

The kind for accessibility visuals and sorting.

