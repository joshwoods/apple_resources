

- PDFKit
-  PDFSelection 

Class

# PDFSelection

A `PDFSelection` object identifies a contiguous or noncontiguous selection of text in a PDF document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
class PDFSelection
```

## Topics

### Initializing a Selection

init(document: PDFDocument)

Returns an empty `PDFSelection` object.

### Getting Information About a Selection

var pages: [PDFPage]

Returns the array of pages contained in the selection.

var string: String?

Returns an `NSString` object representing the text contained in the selection (may contain linefeed characters).

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text contained in the selection (may contain linefeed characters).

func bounds(for: PDFPage) -> CGRect

Returns the bounds of the selection on the specified page.

func selectionsByLine() -> [PDFSelection]

Returns an array of selections, one for each line of text covered by the receiver.

var color: UIColor?

Sets the color used for the drawing of a selection in both active and inactive states.

### Modifying a Selection

func add(PDFSelection)

Adds the specified selection to the receiving selection.

func add([PDFSelection])

Adds the specified array of selections to the receiving selection.

func extend(atEnd: Int)

Extends the selection from its end toward the end of the document.

func extend(atStart: Int)

Extends the selection from its start toward the beginning of the document.

### Managing Selection Drawing

func draw(for: PDFPage, active: Bool)

Calls draw(for:with:active:) with a default value for box parameter.

func draw(for: PDFPage, with: PDFDisplayBox, active: Bool)

Draws the selection relative to the origin of the specified box in page space.

var color: UIColor?

Sets the color used for the drawing of a selection in both active and inactive states.

### Instance Methods

func extendForLineBoundaries()

func numberOfTextRanges(on: PDFPage) -> Int

func range(at: Int, on: PDFPage) -> NSRange

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Content Model

class PDFDocument

An object that represents PDF data or a PDF file and defines methods for writing, searching, and selecting PDF data.

class PDFPage

`PDFPage`, a subclass of `NSObject`, defines methods used to render PDF pages and work with annotations, text, and selections.

class PDFOutline

A `PDFOutline` object is an element in a tree-structured hierarchy that can represent the structure of a PDF document.

