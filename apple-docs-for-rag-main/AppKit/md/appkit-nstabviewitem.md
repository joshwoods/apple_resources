

- AppKit
-  NSTabViewItem 

Class

# NSTabViewItem

An item in a tab view.

macOS

``` source
class NSTabViewItem
```

## Overview

An NSTabViewItem is a convenient way for presenting information in multiple pages. A tab view is usually distinguished by a row of tabs that give the visual appearance of folder tabs. When the user clicks a tab, the tab view displays a view page provided by your application. A tab view keeps a zero-based array of tab view items, one for each tab in the view.

## Topics

### Creating a Tab View Item

init(identifier: Any?)

Performs default initialization for the receiver.

### Working with Labels

func drawLabel(Bool, in: NSRect)

Draws the receiver’s label in `tabRect`, which is the area between the curved end caps.

var label: String

Sets the label text for the receiver to `label`.

func sizeOfLabel(Bool) -> NSSize

Calculates the size of the receiver’s label.

### Checking the Tab Display State

var tabState: NSTabViewItem.State

Returns the current display state of the tab associated with the receiver.

### Assigning an Identifier Object

var identifier: Any?

Sets the receiver’s optional identifier object to `identifier`.

### Setting the Color

var color: NSColor

Sets the background color for content in the view.

### Assigning a View

var view: NSView?

Sets the view associated with the receiver to `view`.

### Setting the Initial First Responder

var initialFirstResponder: NSView?

Sets the initial first responder for the view associated with the receiver (the view that is displayed when a user clicks on the tab) to `view`.

### Accessing the Parent Tab View

var tabView: NSTabView?

Returns the parent tab view for the receiver.

### Getting and Setting Tooltips

var toolTip: String?

Sets the tooltip displayed for the tab view item.

### Constants

enum State

These constants describe the current display state of a tab:

### Initializers

convenience init(viewController: NSViewController)

### Instance Properties

var image: NSImage?

var viewController: NSViewController?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Tab View Interface

class NSTabViewController

A container view controller that manages a tab view interface, which organizes multiple pages of content but displays only one page at a time.

class NSTabView

A multipage interface that displays one page at a time.

