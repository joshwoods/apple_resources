

- UIKit
-  UIBarPositioningDelegate 

Protocol

# UIBarPositioningDelegate

A set of methods that support the positioning of a bar that conforms to the UIBarPositioning protocol.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIBarPositioningDelegate : NSObjectProtocol
```

## Overview

Navigation bars, toolbars, and search bars all have delegates that support the UIBarPositioning protocol. The delegate can use the method of this protocol to specify the bar’s position when that bar is moved to a window. The UINavigationBarDelegate, UISearchBarDelegate, and UIToolbarDelegate protocols extend this protocol to allow for the positioning of those bars on the screen.

## Topics

### Positioning Bars

func position(for: any UIBarPositioning) -> UIBarPosition

Asks the delegate for the position of the specified bar in its new window.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UINavigationBarDelegate
- UISearchBarDelegate
- UIToolbarDelegate

## See Also

### Bars

class UIBarItem

An abstract superclass for items that you can add to a bar that appears at the bottom of the screen.

class UIBarButtonItem

A specialized button for placement on a toolbar, navigation bar, or shortcuts bar.

class UIBarButtonItemGroup

A group of one or more bar button items for placement on a navigation bar or shortcuts bar.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UISearchBar

A specialized view for receiving search-related information from the user.

class UIToolbar

A control that displays one or more buttons along the bottom edge of your interface.

class UITabBar

A control that displays one or more buttons in a tab bar for selecting between different subtasks, views, or modes in an app.

class UITabBarItem

An object that describes an item in a tab bar.

protocol UIBarPositioning

A set of methods for defining the positioning of bars in iOS apps.

