

- UIKit
- UISplitViewController
-  UISplitViewController.Style 

Enumeration

# UISplitViewController.Style

Constants that describe the number of columns the split view interface displays.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
enum Style
```

## Overview

In iOS 14 and later, UISplitViewController supports column-style layouts. A column-style split view controller lets you create an interface with two or three columns by using init(style:) with the appropriate style:

- Use the UISplitViewController.Style.doubleColumn style to create a split view interface with a two-column layout. This style of split view controller manages two child view controllers, placed in the primary and secondary columns.

- Use the UISplitViewController.Style.tripleColumn style to create a split view interface with a three-column layout. This style of split view controller manages three child view controllers, placed in the primary, supplementary, and secondary columns.

Before iOS 14, UISplitViewController supported just one split view interface style with a primary view controller and a secondary view controller. This classic interface style applies to split view controllers created using any other approach than init(style:). Split view controllers with the classic interface have a style of UISplitViewController.Style.unspecified and they don’t respond to any of the column-style APIs introduced in iOS 14 and later.

## Topics

### Constants

case unspecified

The split view interface uses the classic split view style.

case doubleColumn

The split view interface displays two columns.

case tripleColumn

The split view interface displays three columns.

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

### Getting the split view style

var style: UISplitViewController.Style

The style that determines the number of columns that the split view interface displays.

