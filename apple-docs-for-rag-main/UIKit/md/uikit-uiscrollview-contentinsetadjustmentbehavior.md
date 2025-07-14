

- UIKit
- UIScrollView
-  contentInsetAdjustmentBehavior 

Instance Property

# contentInsetAdjustmentBehavior

The behavior for determining the adjusted content offsets.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var contentInsetAdjustmentBehavior: UIScrollView.ContentInsetAdjustmentBehavior { get set }
```

## Discussion

This property specifies how the safe area insets are used to modify the content area of the scroll view. The default value of this property is UIScrollView.ContentInsetAdjustmentBehavior.automatic.

## See Also

### Managing the content inset behavior

var adjustedContentInset: UIEdgeInsets

The insets derived from the content insets and the safe area of the scroll view.

var contentInset: UIEdgeInsets

The custom distance that the content view is inset from the safe area or scroll view edges.

enum ContentInsetAdjustmentBehavior

Constants indicating how safe area insets are added to the adjusted content inset.

func adjustedContentInsetDidChange()

Notifies the scroll view when the adjusted content insets of the scroll view change.

