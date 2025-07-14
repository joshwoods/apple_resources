

- PDFKit
- PDFView
- Configurations
-  Additional Display Configurations 

API Collection

# Additional Display Configurations

Operations for setting up page breaks, a display box, and display direction.

## Topics

### Defining Display Box

var displayBox: PDFDisplayBox

The current style of display box.

### Defining Page Breaks

var displaysPageBreaks: Bool

A Boolean value indicating whether the view is displaying page breaks.

var pageBreakMargins: UIEdgeInsets

The spacing between pages as defined by the top, bottom, left, and right margins.

### Defining Display Direction

var displayDirection: PDFDisplayDirection

The layout direction, either vertical or horizontal, for the given display mode.

var displaysRTL: Bool

The presentation of pages from right-to-left.

## See Also

### Working with Display Modes and Characteristics

var displayMode: PDFDisplayMode

The current display mode.

enum PDFDisplayMode

A wrapper for the chosen display mode constant.

Book Display

Operations to setup a book display for a PDF view.

Graphics Properties

Operations to define the background color, antialiasing, and greeking for a PDF view.

