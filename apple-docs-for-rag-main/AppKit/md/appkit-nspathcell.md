

- AppKit
-  NSPathCell 

Class

# NSPathCell

The user interface of a path control object.

macOS 10.5+

``` source
@MainActor
class NSPathCell
```

## Overview

NSPathCell maintains a collection of NSPathComponentCell objects that represent a particular path to be displayed to the user.

The path shown can be set with the clickedPathComponentCell method. Doing so removes all displayed `NSPathComponentCell` objects and automatically fills the control with `NSPathComponentCell` objects set to have the appropriate icons, display titles, and `NSURL` values for the particular path component they represent. Alternatively, you can fill the control manually by setting the cell array or directly modifying existing cells.

Both an action and double-click action can be set for the path control. To find out what path component cell was clicked in the action, you can read the value of clickedPathComponentCell. When the style is set to NSPathControl.Style.popUp, the action is still sent, and the clickedPathComponentCell value for the represented menu item is correctly set. The clickedPathComponentCell value is valid only when the action is being sent. It is also valid when the keyboard is used to invoke the action.

Automatic animated expansion of partially hidden `NSPathComponentCell` objects happens if you correctly call mouseEntered(with:) and mouseExited(with:) for each `NSPathComponentCell` in the `NSPathCell` object. This is not required if the pathStyle is set to NSPathControl.Style.popUp, or if you wish to not have the animation.

`NSPathCell` supports several path display styles. NSPathControl.Style.standard has a light blue background with arrows indicating the path. NSPathStyleNavigationBar has more defined arrows (chevrons) and looks a little like a segmented button. NSPathControl.Style.popUp looks and works like an NSPopUpButton object to display the full path, or, if the cell is editable, select a new path.

If the cell’s isEditable method returns true (the default), you can drag and drop into the cell to change the value. You can constrain what can be dropped using UTIs (Uniform Type Identifiers) with allowedTypes or the appropriate delegate methods on `NSPathControl`.

If the cell’s isSelectable method returns true (the default), the cell’s contents can automatically be dragged out. The proper UTI, filename, and URL are placed on the pasteboard. You can further control or limit this by using the appropriate delegate methods on `NSPathControl`.

If the cell is editable and has the path style set to NSPathControl.Style.popUp, an additional item in the pop-up menu allows selecting another location. By default, an `NSOpenPanel` object is configured based on the allowed types. The `NSOpenPanel` object can be customized with a delegate method.

## Setting the control size

When setting the controlSize property, `NSPathCell` properly respects the control size for the NSPathControl.Style.standard and NSPathControl.Style.popUp styles. When the control size is set, the new size is propagated to subcells. When the path style is set to NSPathStyleNavigationBar, you cannot change the control size, and it is always set to NSSmallControlSize. Attempting to change the control size when the path style is NSPathStyleNavigationBar causes an assertion. Setting the path style to NSPathStyleNavigationBar forces the control size to be NSSmallControlSize.

## Topics

### Displaying Hidden Components

func mouseEntered(with: NSEvent, frame: NSRect, in: NSView)

Displays the cell component over which the mouse is hovering.

func mouseExited(with: NSEvent, frame: NSRect, in: NSView)

Hides the cell component over which the mouse is hovering.

### Setting the Allowed Types

var allowedTypes: [String]?

Sets the component types allowed in the path when the cell is editable.

### Setting the Control Style

var pathStyle: NSPathControl.Style

Sets the receiver’s path style.

### Setting the Object Value

func setObjectValue((any NSCopying)?)

Sets the receiver’s object value.

### Setting Cell Appearance

var placeholderAttributedString: NSAttributedString?

Sets the value of the placeholder attributed string.

var placeholderString: String?

Returns the placeholder string.

var backgroundColor: NSColor?

Returns the current background color of the receiver.

### Managing Path Components

class var pathComponentCellClass: AnyClass

Returns the class used to create `pathComponentCell` objects when automatically filling up the control.

func rect(of: NSPathComponentCell, withFrame: NSRect, in: NSView) -> NSRect

Returns the current rectangle being displayed for a given path component cell, with respect to a given frame in a given view.

func pathComponentCell(at: NSPoint, withFrame: NSRect, in: NSView) -> NSPathComponentCell?

Returns the cell located at the given point within the given frame of the given view.

var clickedPathComponentCell: NSPathComponentCell?

Sets the value of the path displayed by the receiver.

var pathComponentCells: [NSPathComponentCell]

Sets the array of `NSPathComponentCell` objects currently being displayed.

### Setting the Double-Click Action

var doubleAction: Selector?

Sets the receiver’s double-click action.

### Setting the Path

var url: URL?

Returns the path displayed by the receiver.

var clickedPathComponentCell: NSPathComponentCell?

Sets the value of the path displayed by the receiver.

### Setting the Delegate

var delegate: (any NSPathCellDelegate)?

Sets the receiver’s delegate.

### Constants

enum Style

`NSPathStyle` constants represent the different visual and behavioral styles an `NSPathControl` or `NSPathCell` object can have.

## Relationships

### Inherits From

- NSActionCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSMenuItemValidation
- NSObjectProtocol
- NSOpenSavePanelDelegate
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Cells

protocol NSPathCellDelegate

A set of methods that enable the delegate of a path cell object to customize the Open panel or pop-up menu of a path whose style is set to NSPathControl.Style.popUp.

class NSPathComponentCell

A component of a path.

class NSPathControlItem

