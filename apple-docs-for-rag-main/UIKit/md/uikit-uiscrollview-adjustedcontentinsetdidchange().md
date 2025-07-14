

- UIKit
- UIScrollView
-  adjustedContentInsetDidChange() 

Instance Method

# adjustedContentInsetDidChange()

Notifies the scroll view when the adjusted content insets of the scroll view change.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func adjustedContentInsetDidChange()
```

## See Also

### Managing the content inset behavior

var adjustedContentInset: UIEdgeInsets

The insets derived from the content insets and the safe area of the scroll view.

var contentInset: UIEdgeInsets

The custom distance that the content view is inset from the safe area or scroll view edges.

var contentInsetAdjustmentBehavior: UIScrollView.ContentInsetAdjustmentBehavior

The behavior for determining the adjusted content offsets.

enum ContentInsetAdjustmentBehavior

Constants indicating how safe area insets are added to the adjusted content inset.

