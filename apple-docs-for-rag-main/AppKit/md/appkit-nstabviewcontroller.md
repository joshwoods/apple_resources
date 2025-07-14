

- AppKit
-  NSTabViewController 

Class

# NSTabViewController

A container view controller that manages a tab view interface, which organizes multiple pages of content but displays only one page at a time.

macOS 10.10+

``` source
@MainActor
class NSTabViewController
```

## Overview

Each page of content is managed by a separate child view controller. Navigation between child view controllers is accomplished with the help of an NSTabView object, which the tab view controller manages. When the user selects a new tab, the tab view controller displays the content associated with the associated child view controller, replacing the previous content.

Each tab is represented by an NSTabViewItem object, which contains the name of the tab and stores a pointer to the child view controller that manages the tab’s content. Normally, you configure the tab view items at design time using Interface Builder, but you can also add them programmatically using the methods of this class. Always assign a child view controller to new tab view items before adding those items to the tab view interface.

Another way to add tabs programmatically is to add child view controllers directly to the tab view controller. When you call the addChild(_:) or insertChild(_:at:) method of this class, the tab view controller automatically creates a default NSTabViewItem object for the specified view controller. You can fetch the newly created item using the tabViewItem(for:) method and configure it. Removing a child view controller with the removeChild(at:) method similarly removes the corresponding tab view item.

The tab view controller lazily loads the views associated with each child view controller, creating them only after the corresponding tab is selected. When the tab view controller’s view is first displayed, only the view for the initially selected tab is loaded.

The tabStyle property determines the appearance of the tab controls. A tab view controller can display a segmented control or display tabs in the window’s toolbar. You can also provide your own control for displaying tabs. The tab view controller automatically coordinates interactions between designated control and the corresponding tabView object.

## Topics

### Configuring the Tab View

var tabStyle: NSTabViewController.TabStyle

The style used to display the tabs.

var tabView: NSTabView

The tab view that manages the views of the interface.

var transitionOptions: NSViewController.TransitionOptions

The animation options to use when switching between tabs.

var canPropagateSelectedChildViewControllerTitle: Bool

A Boolean value indicating whether the tab view controller gets its title from the selected child view controller.

### Managing Tab View Items

var tabViewItems: [NSTabViewItem]

The array of tab view items used to manage each of the child view controllers.

func tabViewItem(for: NSViewController) -> NSTabViewItem?

Returns the tab view item for the specified child view controller.

func addTabViewItem(NSTabViewItem)

Adds the specified tab to the end of the tab view controller’s list of tabs.

func insertTabViewItem(NSTabViewItem, at: Int)

Inserts a tab view into the tab view controller’s list of tabs.

func removeTabViewItem(NSTabViewItem)

Removes the specified tab view item from the tab view controller.

var selectedTabViewItemIndex: Int

The index of the selected tab.

### Responding to Tab View Events

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

func tabView(NSTabView, shouldSelect: NSTabViewItem?) -> Bool

Asks the tab view controller if the specified tab should be selected.

func tabView(NSTabView, willSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab is about to be selected.

func tabView(NSTabView, didSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab was selected.

### Responding to Toolbar Events

func toolbar(NSToolbar, itemForItemIdentifier: NSToolbarItem.Identifier, willBeInsertedIntoToolbar: Bool) -> NSToolbarItem?

Returns the toolbar item for the specified identifier.

func toolbarAllowedItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Returns the array of identifier strings for the allowed toolbar items.

func toolbarDefaultItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Returns the array of identifier strings for the default toolbar items.

func toolbarSelectableItemIdentifiers(NSToolbar) -> [NSToolbarItem.Identifier]

Returns the array of identifier strings for the selectable toolbar items

### Constants

enum TabStyle

Tab control style options for a tab view controller.

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTabViewDelegate
- NSToolbarDelegate
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Tab View Interface

class NSTabView

A multipage interface that displays one page at a time.

class NSTabViewItem

An item in a tab view.

