

- AppKit
-  NSTabView 

Class

# NSTabView

A multipage interface that displays one page at a time.

macOS

``` source
@MainActor
class NSTabView
```

## Overview

A tab view contains a row of tabs that give the appearance of folder tabs, as shown in the Figure 1. The user selects the desired page by clicking the appropriate tab or using the arrow keys to move between pages. Each page displays a view hierarchy provided by your app.

## Topics

### Handling the Selection of Tabs

var delegate: (any NSTabViewDelegate)?

The tab view’s delegate.

protocol NSTabViewDelegate

The `NSTabViewDelegate` protocol defines the optional methods implemented by delegates of `NSTabView` objects.

### Adding and Removing Tabs

func addTabViewItem(NSTabViewItem)

Adds the specified tab item.

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts the specified item into the tab view’s array of tab view items at the specified index.

func removeTabViewItem(NSTabViewItem)

Removes the specified item from the tab view’s array of tab view items.

### Accessing Tabs

func indexOfTabViewItem(NSTabViewItem) -> Int

Returns the index of the specified item in the tab view.

func indexOfTabViewItem(withIdentifier: Any) -> Int

Returns the index of the item that matches the specified identifier or `NSNotFound` if the item is not found.

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

func tabViewItem(at: Int) -> NSTabViewItem

Returns the tab view item at `index` in the tab view’s array of items.

var tabViewItems: [NSTabViewItem]

The tab view’s array of tab view items.

### Configuring the Tab Attributes

var tabViewType: NSTabView.TabType

The tab type to display the tabs.

enum TabType

These constants specify the tab view’s type as used by the tabViewType property.

var tabPosition: NSTabView.TabPosition

enum TabPosition

var tabViewBorderType: NSTabView.TabViewBorderType

enum TabViewBorderType

### Selecting a Tab

func selectFirstTabViewItem(Any?)

This action method selects the first tab view item.

func selectLastTabViewItem(Any?)

This action method selects the last tab view item.

func selectNextTabViewItem(Any?)

This action method selects the next tab view item in the sequence.

func selectPreviousTabViewItem(Any?)

This action method selects the previous tab view item in the sequence.

func selectTabViewItem(NSTabViewItem?)

Selects the specified tab view item.

func selectTabViewItem(at: Int)

Selects the tab view item specified by `index`.

func selectTabViewItem(withIdentifier: Any)

Selects the tab view item specified by `identifier`.

var selectedTabViewItem: NSTabViewItem?

The tab view item for the currently selected tab.

func takeSelectedTabViewItemFromSender(Any?)

Sets the selected tab view item to the selected item obtained from the sender.

### Modifying the Font

var font: NSFont

The font used for the tab view’s label text.

### Modifying Controls Tint

var controlTint: NSControlTint

The tab view’s control tint.

Deprecated

### Manipulating the Background

var drawsBackground: Bool

A Boolean value that indicates if the tab view draws a background color when its type is `NSNoTabsNoBorder`.

### Determining the Size

var minimumSize: NSSize

The minimum size necessary for the tab view to display tabs in a useful way.

var contentRect: NSRect

The rectangle describing the content area of the tab view.

var controlSize: NSControl.ControlSize

The size of the tab view.

### Truncating Tab Labels

var allowsTruncatedLabels: Bool

A Boolean value that indicates if the tab view allows truncating for labels that don’t fit on a tab.

### Event Handling

func tabViewItem(at: NSPoint) -> NSTabViewItem?

Returns the tab view item at the specified point.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Tab View Interface

class NSTabViewController

A container view controller that manages a tab view interface, which organizes multiple pages of content but displays only one page at a time.

class NSTabViewItem

An item in a tab view.

