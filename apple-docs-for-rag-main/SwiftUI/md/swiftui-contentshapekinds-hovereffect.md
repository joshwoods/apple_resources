

- SwiftUI
- ContentShapeKinds
-  hoverEffect 

Type Property

# hoverEffect

The kind for hover effects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 18.0+visionOS 1.0+

``` source
static let hoverEffect: ContentShapeKinds
```

## Discussion

When using this kind, only the preview shape is affected. To control the shape used to hit-test and start the effect, use the `interaction` kind.

On tvOS, this is used to define the shape of any hover effect applied to focusable and hoverable controls, for example button border or clipping shapes.

This kind does not affect the `onHover` modifier.

## See Also

### Getting shape kinds

static let interaction: ContentShapeKinds

The kind for hit-testing and accessibility.

static let dragPreview: ContentShapeKinds

The kind for drag and drop previews.

static let contextMenuPreview: ContentShapeKinds

The kind for context menu previews.

static let focusEffect: ContentShapeKinds

The kind for the focus effect.

static let accessibility: ContentShapeKinds

The kind for accessibility visuals and sorting.

