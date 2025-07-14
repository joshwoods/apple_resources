

- UIKit
- UIScrollView
-  automaticallyAdjustsScrollIndicatorInsets 

Instance Property

# automaticallyAdjustsScrollIndicatorInsets

A Boolean value that indicates whether the system automatically adjusts the scroll indicator insets.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var automaticallyAdjustsScrollIndicatorInsets: Bool { get set }
```

## Discussion

The default value is true.

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

func flashScrollIndicators()

Displays the scroll indicators momentarily.

func withScrollIndicatorsShown(forContentOffsetChanges: () -> Void)

Displays the scroll indicators during updates to the scroll view’s content offset.

var refreshControl: UIRefreshControl?

The refresh control associated with the scroll view.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

