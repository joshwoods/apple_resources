

- AppKit
-  NSTableHeaderCell 

Class

# NSTableHeaderCell

An object that a table header view uses to draw the content of the column headers.

macOS

``` source
@MainActor
class NSTableHeaderCell
```

## Overview

Subclasses of the `NSTableHeaderCell` class can override the drawInterior(withFrame:in:), edit(withFrame:in:editor:delegate:event:), and highlight(_:withFrame:in:) methods to change the way headers appear. This specific subclass is responsible for drawing the sort indicators. See the NSCell class specification for information on overriding these methods.

See the NSTableView and NSTableHeaderCell for more information.

## Topics

### Drawing Sorting Indicators

func drawSortIndicator(withFrame: NSRect, in: NSView, ascending: Bool, priority: Int)

Draws a sorting indicator given a cell frame contained inside a view.

func sortIndicatorRect(forBounds: NSRect) -> NSRect

Returns the location to display the sorting indicator given `theRect`.

## Relationships

### Inherits From

- NSTextFieldCell

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
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Rows and Columns

class NSTableHeaderView

An object that draws headers over a table view’s columns and handles mouse events in those headers.

class NSTableRowView

The view shown for a row in a table view.

class NSTableColumn

The display characteristics and identifier for a column in a table view.

class NSTableViewRowAction

A single action to present when the user swipes horizontally on a table row.

struct ResizingOptions

