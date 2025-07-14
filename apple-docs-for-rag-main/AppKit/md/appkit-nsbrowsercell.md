

- AppKit
-  NSBrowserCell 

Class

# NSBrowserCell

The user interface of a browser.

macOS

``` source
@MainActor
class NSBrowserCell
```

## Overview

The NSBrowserCell class is the subclass of NSCell used by default to display data in the columns of an NSBrowser object. (Each column contains an NSMatrix object filled with NSBrowserCell objects.)

## Topics

### Getting Browser Cell Information

class var branchImage: NSImage?

Returns the default image for branch cells in a browser.

class var highlightedBranchImage: NSImage?

Returns the default image for branch browser cells that are highlighted.

### Configuring Browser Cells

var image: NSImage?

The browser cell’s image.

var alternateImage: NSImage?

The browser cell’s image for the highlighted state.

### Managing Browser Cell State

func reset()

Unhighlights the receiver and unsets its state.

func set()

Highlights the receiver and sets its state.

var isLeaf: Bool

A Boolean that indicates whether the browser cell is a leaf or a branch cell.

var isLoaded: Bool

A Boolean that indicates whether the cell is ready to display.

func highlightColor(in: NSView) -> NSColor?

Returns the highlight color that the receiver wants to display.

### Initializers

init(coder: NSCoder)

init(imageCell: NSImage?)

init(textCell: String)

## Relationships

### Inherits From

- NSCell

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

