

- UIKit
- UINavigationBar
-  titleTextAttributes 

Instance Property

# titleTextAttributes

Display attributes for the bar’s title text.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var titleTextAttributes: [NSAttributedString.Key : Any]? { get set }
```

## Discussion

You can specify the font, text color, text shadow color, and text shadow offset for the title in the text attributes dictionary, using the text attribute keys described in NSAttributedString.Key.

## See Also

### Configuring the title

var largeTitleTextAttributes: [NSAttributedString.Key : Any]?

Display attributes for the bar’s large title text.

func titleVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the title’s vertical position adjustment for given bar metrics.

func setTitleVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the title’s vertical position adjustment for given bar metrics.

