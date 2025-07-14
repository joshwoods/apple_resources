

- UIKit
- UIVisualEffectView
-  contentView 

Instance Property

# contentView

A view object that can have a visual effect view added to it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentView: UIView { get }
```

## Discussion

Add subviews to the contentView and not to UIVisualEffectView directly.

## See Also

### Retrieving view information

var effect: UIVisualEffect?

The visual effect provided by the view.

