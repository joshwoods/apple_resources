

- UIKit
- UIScrollView
-  contentInset 

Instance Property

# contentInset

The custom distance that the content view is inset from the safe area or scroll view edges.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentInset: UIEdgeInsets { get set }
```

## Discussion

Use this property to extend the space between your content and the edges of the content view. The unit of size is points. The default value is zero.

By default, UIKit automatically adjusts the content inset to account for overlapping bars. You use this property to extend that distance even further, perhaps to accommodate your own custom content. Get the total adjustment — the safe area plus your custom insets — using the adjustedContentInset property. To change how the safe area is applied, modify the contentInsetAdjustmentBehavior property.

## See Also

### Managing the content inset behavior

var adjustedContentInset: UIEdgeInsets

The insets derived from the content insets and the safe area of the scroll view.

var contentInsetAdjustmentBehavior: UIScrollView.ContentInsetAdjustmentBehavior

The behavior for determining the adjusted content offsets.

enum ContentInsetAdjustmentBehavior

Constants indicating how safe area insets are added to the adjusted content inset.

func adjustedContentInsetDidChange()

Notifies the scroll view when the adjusted content insets of the scroll view change.

