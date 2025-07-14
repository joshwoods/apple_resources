

- AppKit
-  NSTableCellView 

Class

# NSTableCellView

A reusable container view shown for a particular cell in a table view that uses rows for content.

macOS 10.7+

``` source
@MainActor
class NSTableCellView
```

## Overview

The imageView and textField properties are connected in Interface Builder. Additional properties can be added by subclassing NSTableCellView and adding the required properties and connecting them programmatically or in Interface Builder.

The `objectValue` is used when setting the value of the view cell by the tableView(_:objectValueFor:row:) method in the NSTableViewDataSource. If you use your own custom view cells that are not based on NSTableCellView you should implement this property in order to be able to receive changes to cell values.

## Topics

### Represented Object

var objectValue: Any?

The object that represents the cell data.

### Displayed Items

var imageView: NSImageView?

Image displayed by the cell.

var textField: NSTextField?

Text displayed by the cell.

### Getting and Setting the Background Style

var backgroundStyle: NSView.BackgroundStyle

This property is automatically set by the enclosing row view to let this view know what its background looks like.

### Getting and Setting the Row Size Style

var rowSizeStyle: NSTableView.RowSizeStyle

Returns the row size style.

### Dragging Images

var draggingImageComponents: [NSDraggingImageComponent]

Returns dragging images for the cell.

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

### Views

class NSTableView

A set of related records, displayed in rows that represent individual records and columns that represent the attributes of those records.

