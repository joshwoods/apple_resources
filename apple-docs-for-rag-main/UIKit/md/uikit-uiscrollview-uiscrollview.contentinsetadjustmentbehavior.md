

- UIKit
- UIScrollView
-  UIScrollView.ContentInsetAdjustmentBehavior 

Enumeration

# UIScrollView.ContentInsetAdjustmentBehavior

Constants indicating how safe area insets are added to the adjusted content inset.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
enum ContentInsetAdjustmentBehavior
```

## Topics

### Enumeration Cases

case always

Always include the safe area insets in the content adjustment.

case automatic

Automatically adjust the scroll view insets.

case never

Do not adjust the scroll view insets.

case scrollableAxes

Adjust the insets only in the scrollable directions.

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

### Managing the content inset behavior

var adjustedContentInset: UIEdgeInsets

The insets derived from the content insets and the safe area of the scroll view.

var contentInset: UIEdgeInsets

The custom distance that the content view is inset from the safe area or scroll view edges.

var contentInsetAdjustmentBehavior: UIScrollView.ContentInsetAdjustmentBehavior

The behavior for determining the adjusted content offsets.

func adjustedContentInsetDidChange()

Notifies the scroll view when the adjusted content insets of the scroll view change.

