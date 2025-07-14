

- PDFKit
-  PDFDisplayMode 

Enumeration

# PDFDisplayMode

A wrapper for the chosen display mode constant.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
enum PDFDisplayMode
```

## Topics

### Constants

case singlePage

A display mode where the document displays one page at a time horizontally and vertically.

case singlePageContinuous

A display mode where the document displays in continuous mode vertically, with single-page width horizontally.

case twoUp

A display mode where the document displays two pages side-by-side.

case twoUpContinuous

A display mode where the document displays in continuous mode vertically and displays two pages side-by-side horizontally.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with Display Modes and Characteristics

var displayMode: PDFDisplayMode

The current display mode.

Additional Display Configurations

Operations for setting up page breaks, a display box, and display direction.

Book Display

Operations to setup a book display for a PDF view.

Graphics Properties

Operations to define the background color, antialiasing, and greeking for a PDF view.

