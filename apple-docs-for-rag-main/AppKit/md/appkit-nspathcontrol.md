

- AppKit
-  NSPathControl 

Class

# NSPathControl

A display of a file system path or virtual path information.

macOS 10.5+

``` source
@MainActor
class NSPathControl
```

## Overview

The NSPathControl class uses NSPathCell to implement its user interface. NSPathControl provides cover methods for most NSPathCell methods—the cover method simply invokes the corresponding cell method. See also NSPathComponentCell, which represents individual components of the path, and two associated protocols: NSPathCellDelegate and NSPathControlDelegate.

NSPathControl has three styles represented by the NSPathControl.Style enumeration constants NSPathControl.Style.standard, NSPathStyleNavigationBar, and NSPathControl.Style.popUp. The represented path can be a file system path or any other type of path leading through a sequence of nodes or components, as defined by the programmer.

NSPathControl automatically supports drag and drop, which can be further customized via delegate methods. To accept drag and drop, NSPathControl calls registerForDraggedTypes(_:) with NSFilenamesPboardType and NSURLPboardType. When the URL value in the NSPathControl object changes because of an automatic drag and drop operation or the user selecting a new path via the open panel, the action is sent. In OS X v10.5 the value returned by clickedPathComponentCell() is `nil`, in macOS 10.6 and later, clickedPathComponentCell() returns the clicked cell.

## Topics

### Setting the Control Style

var pathStyle: NSPathControl.Style

The receiver’s path style.

### Setting the Background Color

var backgroundColor: NSColor?

The receiver’s background color.

### Managing Path Components

func clickedPathComponentCell() -> NSPathComponentCell?

Returns the clicked cell.

Deprecated

func pathComponentCells() -> [NSPathComponentCell]

Returns an array of the `NSPathComponentCell` objects currently being displayed.

Deprecated

func setPathComponentCells([NSPathComponentCell])

Sets the array of `NSPathComponentCell` objects currently being displayed.

Deprecated

### Setting the Double-Click Action

var doubleAction: Selector?

The receiver’s double-click action method.

### Setting the Path

var url: URL?

The path value displayed by the receiver.

### Setting the Delegate

var delegate: (any NSPathControlDelegate)?

The receiver’s delegate.

### Setting the Drag Operation Mask

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

### Setting Popup Menu

var menu: NSMenu?

The menu that is used for the path control’s cells.

### Instance Properties

var allowedTypes: [String]?

var clickedPathItem: NSPathControlItem?

var isEditable: Bool

var pathItems: [NSPathControlItem]

var placeholderAttributedString: NSAttributedString?

var placeholderString: String?

### Enumerations

enum Style

`NSPathStyle` constants represent the different visual and behavioral styles an `NSPathControl` or `NSPathCell` object can have.

## Relationships

### Inherits From

- NSControl

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

