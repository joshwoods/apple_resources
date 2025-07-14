

- UIKit
- UIScrollView
-  refreshControl 

Instance Property

# refreshControl

The refresh control associated with the scroll view.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var refreshControl: UIRefreshControl? { get set }
```

## See Also

### Managing the scroll indicator and refresh control

var indicatorStyle: UIScrollView.IndicatorStyle

The style of the scroll indicators.

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

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

