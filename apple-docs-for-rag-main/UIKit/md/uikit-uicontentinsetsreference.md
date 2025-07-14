

- UIKit
-  UIContentInsetsReference 

Enumeration

# UIContentInsetsReference

Constants that describe the reference point of the content insets.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
enum UIContentInsetsReference
```

## Topics

### Constants

case automatic

Content insets use the system default reference point.

case none

Content insets don’t have a reference point in relation to other insets.

case safeArea

Content insets use a reference point in relation to the safe area.

case layoutMargins

Content insets use a reference point in relation to the layout margins.

case readableContent

Content insets use a reference point in relation to the readable content guide.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring section spacing

var interGroupSpacing: CGFloat

The amount of space between the groups in the section.

var contentInsets: NSDirectionalEdgeInsets

The amount of space between the content of the section and its boundaries.

var contentInsetsReference: UIContentInsetsReference

The boundary to reference when defining content insets.

var supplementaryContentInsetsReference: UIContentInsetsReference

The reference boundary for content insets on boundary supplementary items.

