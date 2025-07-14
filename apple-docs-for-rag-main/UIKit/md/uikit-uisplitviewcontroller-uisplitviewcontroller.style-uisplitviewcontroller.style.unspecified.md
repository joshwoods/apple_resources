

- UIKit
- UISplitViewController
- UISplitViewController.Style
-  UISplitViewController.Style.unspecified 

Case

# UISplitViewController.Style.unspecified

The split view interface uses the classic split view style.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0–1.0Deprecated

``` source
case unspecified
```

## Discussion

A split view controller with this style represents a classic split view controller created using any other approach than init(style:). You cannot create a split view controller with a style of UISplitViewController.Style.unspecified using this initializer.

Split view controllers with this style don’t support any column-style APIs, such as setViewController(_:for:).

## See Also

### Constants

case doubleColumn

The split view interface displays two columns.

case tripleColumn

The split view interface displays three columns.

