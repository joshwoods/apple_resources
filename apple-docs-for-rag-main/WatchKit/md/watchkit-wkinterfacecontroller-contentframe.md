

- WatchKit
- WKInterfaceController
-  contentFrame 

Instance Property

# contentFrame

The frame rectangle used to display your app’s content.

watchOS 2.0+

``` source
@MainActor
var contentFrame: CGRect { get }
```

## Discussion

The rectangle in this property is specified in points. This rectangle may be different than the screen bounds.

## See Also

### Respecting safe areas and layout margins

var contentSafeAreaInsets: UIEdgeInsets

Insets that define the area where it’s safe to display content on the screen.

var systemMinimumLayoutMargins: NSDirectionalEdgeInsets

Leading and trailing insets that represent the minimum layout margins for text elements.

