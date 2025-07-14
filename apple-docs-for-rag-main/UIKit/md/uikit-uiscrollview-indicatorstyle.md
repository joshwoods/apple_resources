

- UIKit
- UIScrollView
-  indicatorStyle 

Instance Property

# indicatorStyle

The style of the scroll indicators.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var indicatorStyle: UIScrollView.IndicatorStyle { get set }
```

## Discussion

The default style is UIScrollView.IndicatorStyle.default. See UIScrollView.IndicatorStyle for descriptions of these constants.

## See Also

### Managing the scroll indicator and refresh control

enum IndicatorStyle

Defines constants that represent the styles of the scroll indicators.

var showsHorizontalScrollIndicator: Bool

A Boolean value that controls whether the horizontal scroll indicator is visible.

var showsVerticalScrollIndicator: Bool

A Boolean value that controls whether the vertical scroll indicator is visible.

var horizontalScrollIndicatorInsets: UIEdgeInsets

The horizontal distance the scroll indicators are inset from the edge of the scroll view.

var verticalScrollIndicatorInsets: UIEdgeInsets

The vertical distance the scroll indicators are inset from the edge of the scroll view.

var automaticallyAdjustsScrollIndicatorInsets: Bool

A Boolean value that indicates whether the system automatically adjusts the scroll indicator insets.

func flashScrollIndicators()

Displays the scroll indicators momentarily.

func withScrollIndicatorsShown(forContentOffsetChanges: () -> Void)

Displays the scroll indicators during updates to the scroll view’s content offset.

var refreshControl: UIRefreshControl?

The refresh control associated with the scroll view.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

