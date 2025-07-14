

- UIKit
- UIScrollView
-  UIScrollView.IndicatorStyle 

Enumeration

# UIScrollView.IndicatorStyle

Defines constants that represent the styles of the scroll indicators.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum IndicatorStyle
```

## Overview

You use these constants to set the value of the indicatorStyle style.

## Topics

### Constants

case `default`

The default style of scroll indicator, which is black with a white border.

case black

A style of indicator which is black and smaller than the default style.

case white

A style of indicator is white and smaller than the default style.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the scroll indicator and refresh control

var indicatorStyle: UIScrollView.IndicatorStyle

The style of the scroll indicators.

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

