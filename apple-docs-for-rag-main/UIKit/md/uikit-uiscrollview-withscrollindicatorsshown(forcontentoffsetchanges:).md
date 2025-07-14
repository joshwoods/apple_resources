

- UIKit
- UIScrollView
-  withScrollIndicatorsShown(forContentOffsetChanges:) 

Instance Method

# withScrollIndicatorsShown(forContentOffsetChanges:)

Displays the scroll indicators during updates to the scroll view’s content offset.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func withScrollIndicatorsShown(forContentOffsetChanges changes: () -> Void)
```

## Parameters 

`changes`  

A block that changes the scroll view’s content offset.

## Discussion

The scroll view displays the scroll indicator for an axis if the content offset changes along that axis; otherwise, the scroll indicator for that axis remains hidden. For example, if you update the content offset horizontally in the `changes` block, the scroll view shows the horizontal scroll indicator but not the vertical scroll indicator.

If you animate changes to the content offset in the `changes` block, the scroll view displays its scroll indicators in their original locations, animates them to the destination locations, then fades them out. Otherwise, the scroll view displays its scroll indicators in the destination locations, then fades them out.

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

var refreshControl: UIRefreshControl?

The refresh control associated with the scroll view.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

