

- UIKit
-  UINavigationBarDelegate 

Protocol

# UINavigationBarDelegate

Methods that a navigation bar calls before and after it modifies its stack of navigation items.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UINavigationBarDelegate : UIBarPositioningDelegate
```

## Overview

The UINavigationBarDelegate protocol defines optional methods that a UINavigationBar delegate implements to update its views when items push or pop from the stack. The navigation bar represents only the bar at the top of the screen, not the view below. It’s the application’s responsibility to implement the behavior when the top item changes.

You can control whether a navigation bar pushes an item on or pops an item from the stack by implementing the navigationBar(_:shouldPush:) and navigationBar(_:shouldPop:) methods. These methods return true if the action is allowed; otherwise, false.

The screen always reflects the top item on the navigation bar. You implement the navigationBar(_:didPush:) method to update the view below the navigation bar to reflect the new item. Similarly, you implement the navigationBar(_:didPop:) method to replace the view below the navigation bar.

## Topics

### Pushing items

func navigationBar(UINavigationBar, shouldPush: UINavigationItem) -> Bool

Returns a Boolean value indicating whether the navigation bar should push an item.

func navigationBar(UINavigationBar, didPush: UINavigationItem)

Tells the delegate that an item was pushed onto the navigation bar.

### Popping items

func navigationBar(UINavigationBar, shouldPop: UINavigationItem) -> Bool

Returns a Boolean value indicating whether the navigation bar should pop an item.

func navigationBar(UINavigationBar, didPop: UINavigationItem)

Tells the delegate that an item was popped from the navigation bar.

### Building with Mac Catalyst

func navigationBarNSToolbarSection(UINavigationBar) -> UINavigationBar.NSToolbarSection

Asks the delegate which section of the toolbar to host the navigation bar in.

## Relationships

### Inherits From

- NSObjectProtocol
- UIBarPositioningDelegate

## See Also

### Responding to navigation bar changes

var delegate: (any UINavigationBarDelegate)?

The navigation bar’s delegate object.

