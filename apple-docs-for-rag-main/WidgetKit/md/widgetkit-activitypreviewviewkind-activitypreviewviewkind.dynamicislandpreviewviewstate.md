

- WidgetKit
- ActivityPreviewViewKind
-  ActivityPreviewViewKind.DynamicIslandPreviewViewState 

Enumeration

# ActivityPreviewViewKind.DynamicIslandPreviewViewState

Values that represent the different presentations of a Live Activity in the Dynamic Island for use in Xcode previews.

iOS 16.2+iPadOS 16.2+Mac Catalyst 16.2+

``` source
@preconcurrency
enum DynamicIslandPreviewViewState
```

## Topics

### Dynamic Island presentations

case compact

The presentation of a Live Activity in the Dynamic Island that shows both the compactLeading and compactTrailing views combined.

case minimal

The minimal presentation of a Live Activity in the Dynamic Island.

case expanded

The expanded presentation of a Live Activity in the Dynamic Island.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Live Activity preview types

case content

The Live Activity presentation that appears on the Lock Screen and as a banner on devices that don’t support the Dynamic Island.

case dynamicIsland(ActivityPreviewViewKind.DynamicIslandPreviewViewState)

The Live Activity presentation that appears in the Dynamic Island.

