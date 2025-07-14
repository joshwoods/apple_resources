

- WatchKit
- WKInterfaceController
-  systemMinimumLayoutMargins 

Instance Property

# systemMinimumLayoutMargins

Leading and trailing insets that represent the minimum layout margins for text elements.

watchOS 5.0+

``` source
@MainActor
var systemMinimumLayoutMargins: NSDirectionalEdgeInsets { get }
```

## Discussion

The 40 mm and 44 mm watches have rounded corners. As a result, the items in the status bar do not extend all the way to the edge of the screen.

The system provides the minimum layout margins to help you align your text content with the status bar. The system’s built-in containers and controls take the minimum layout margins into account automatically when laying out your interface; however, if you build a custom user interface with SpriteKit or SceneKit, check the contentSafeAreaInsets and systemMinimumLayoutMargins, and lay out your interface accordingly.

The system sets the systemMinimumLayoutMargins property just before it calls the controller’s didAppear() method. Before calling didAppear(), the property may contain an invalid value.

## See Also

### Respecting safe areas and layout margins

var contentSafeAreaInsets: UIEdgeInsets

Insets that define the area where it’s safe to display content on the screen.

var contentFrame: CGRect

The frame rectangle used to display your app’s content.

