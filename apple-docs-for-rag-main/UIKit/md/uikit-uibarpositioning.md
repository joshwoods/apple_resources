

- UIKit
-  UIBarPositioning 

Protocol

# UIBarPositioning

A set of methods for defining the positioning of bars in iOS apps.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIBarPositioning : NSObjectProtocol
```

## Overview

Bars can be positioned at the bottom of their enclosing view, at the top of their enclosing view, or at both the top of their enclosing view and also the top of the screen. In this last case, the bar will abut the status bar displayed by the system. Bars in this position need to have their background extend above their own frame to the top of the screen. This allows the background to show through the status bar.

The classes that implement bars have paired methods to set a background for a given position and set of metrics. These are named similar to the following: backgroundImage(for:barMetrics:) and setBackgroundImage(_:for:barMetrics:). Use these methods to set an appropriate background image for the different possible bar positions and metrics.

## Topics

### Accessing the bar position

var barPosition: UIBarPosition

The position of the bar.

**Required**

### Constants

enum UIBarMetrics

Constants to specify metrics to use for appearance.

enum UIBarPosition

Constants to identify the position of a bar.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UINavigationBar
- UISearchBar
- UIToolbar

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

protocol UIBarPositioningDelegate

A set of methods that support the positioning of a bar that conforms to the UIBarPositioning protocol.

