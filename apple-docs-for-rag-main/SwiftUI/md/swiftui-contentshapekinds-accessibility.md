

- SwiftUI
- ContentShapeKinds
-  accessibility 

Type Property

# accessibility

The kind for accessibility visuals and sorting.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let accessibility: ContentShapeKinds
```

## Discussion

Setting a content shape with this kind causes the accessibility frame and path of the view’s underlying accessibility element to match the shape without adjusting the hit-testing shape, updating the visual focus ring that assistive apps, such as VoiceOver, draw, as well as how the element is sorted. Updating the accessibility shape is only required if the shape or size used to hit-test significantly diverges from the visual shape of the view.

To control the shape for accessibility and hit-testing, use the `interaction` kind.

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

static let hoverEffect: ContentShapeKinds

The kind for hover effects.

