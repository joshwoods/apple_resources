

- WatchKit
- WKInterfaceController
-  contentSafeAreaInsets 

Instance Property

# contentSafeAreaInsets

Insets that define the area where it’s safe to display content on the screen.

watchOS 5.0+

``` source
@MainActor
var contentSafeAreaInsets: UIEdgeInsets { get }
```

## Discussion

The 40 mm and 44 mm watches have rounded corners that may clip content that extends to the edge of the screen. The content-safe area defines the region below the status bar that avoids the rounded corners.

The system’s built-in containers and controls automatically use the content-safe area insets; however, if you build a custom user interface with SpriteKit or SceneKit, you should check the contentSafeAreaInsets and systemMinimumLayoutMargins, and lay out your interface accordingly.

The system sets contentSafeAreaInsets property just before it calls the controller’s didAppear() method. Before didAppear(), the property may contain an invalid value.

## See Also

### Respecting safe areas and layout margins

var systemMinimumLayoutMargins: NSDirectionalEdgeInsets

Leading and trailing insets that represent the minimum layout margins for text elements.

var contentFrame: CGRect

The frame rectangle used to display your app’s content.

