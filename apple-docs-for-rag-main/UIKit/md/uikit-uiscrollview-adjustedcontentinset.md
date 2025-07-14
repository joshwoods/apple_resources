

- UIKit
- UIScrollView
-  adjustedContentInset 

Instance Property

# adjustedContentInset

The insets derived from the content insets and the safe area of the scroll view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var adjustedContentInset: UIEdgeInsets { get }
```

## Discussion

Use this property to obtain the adjusted area in which to draw content. The contentInsetAdjustmentBehavior property determines whether the safe area insets are included in the adjustment. The safe area insets are then added to the values in the contentInset property to obtain the final value of this property.

## See Also

### Managing the content inset behavior

var contentInset: UIEdgeInsets

The custom distance that the content view is inset from the safe area or scroll view edges.

var contentInsetAdjustmentBehavior: UIScrollView.ContentInsetAdjustmentBehavior

The behavior for determining the adjusted content offsets.

enum ContentInsetAdjustmentBehavior

Constants indicating how safe area insets are added to the adjusted content inset.

func adjustedContentInsetDidChange()

Notifies the scroll view when the adjusted content insets of the scroll view change.

