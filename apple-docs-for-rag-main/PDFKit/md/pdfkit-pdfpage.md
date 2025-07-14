

- PDFKit
-  PDFPage 

Class

# PDFPage

`PDFPage`, a subclass of `NSObject`, defines methods used to render PDF pages and work with annotations, text, and selections.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
class PDFPage
```

## Mentioned in 

Adding Custom Graphics to a PDF

## Overview

`PDFPage` objects are flexible and powerful. With them you can render PDF content onscreen or to a printer, add annotations, count characters, define selections, and get the textual content of a page as an `NSString` object.

Your application instantiates a `PDFPage` object by asking for one from a `PDFDocument` object.

For simple display and navigation of PDF documents within your application, you don’t need to use `PDFPage`. You need only use `PDFView`.

## Topics

### Initializing a Page

convenience init?(image: UIImage)

Creates a new `PDFPage` object and initializes it with the specified `NSImage` object.

### Getting Information About a Page

var document: PDFDocument?

Returns the `PDFDocument` object with which the page is associated.

var label: String?

Returns the label for the page.

func bounds(for: PDFDisplayBox) -> CGRect

Returns the bounds for the specified PDF display box.

func setBounds(CGRect, for: PDFDisplayBox)

Sets the bounds for the specified box.

var rotation: Int

Sets the rotation angle for the page in degrees.

### Working with Annotations

var annotations: [PDFAnnotation]

Returns an array containing the page’s annotations.

var displaysAnnotations: Bool

Returns a Boolean value indicating whether annotations are displayed for the page.

func addAnnotation(PDFAnnotation)

Adds the specified annotation object to the page.

func removeAnnotation(PDFAnnotation)

Removes the specified annotation from the page.

func annotation(at: CGPoint) -> PDFAnnotation?

Returns the annotation, if there is one, at the specified point.

### Rendering Pages

func draw(with: PDFDisplayBox)

Draws the page within the specified box.

Deprecated

func transformContext(for: PDFDisplayBox)

Transforms the current context, given the specified box.

Deprecated

### Working with Textual Content

var numberOfCharacters: Int

Returns the number of characters on the page, including whitespace characters.

var string: String?

Returns an `NSString` object representing the text on the page.

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text on the page.

func characterBounds(at: Int) -> CGRect

Returns the bounds, in page space, of the character at the specified index.

func characterIndex(at: CGPoint) -> Int

Returns the character index value for the specified point in page space.

### Working with Selections

func selection(for: CGRect) -> PDFSelection?

Returns the text enclosed within the specified rectangle, expressed in page (user) coordinates.

func selectionForWord(at: CGPoint) -> PDFSelection?

Returns the whole word that includes the specified point.

func selectionForLine(at: CGPoint) -> PDFSelection?

Returns the whole line of text that includes the specified point.

func selection(from: CGPoint, to: CGPoint) -> PDFSelection?

Returns the text between the two specified points in page space.

func selection(for: NSRange) -> PDFSelection?

Returns the text contained within the specified range.

### Supporting Types

enum PDFDisplayBox

The following box types may be used with `PDFPage` drawing and bounds-setting methods. See the Adobe PDF Specification for more information on box types, units, and coordinate systems.

enum PDFDisplayDirection

### Type Aliases

struct ImageInitializationOption

### Initializers

init()

init?(image: UIImage, options: [PDFPage.ImageInitializationOption : Any])

### Instance Properties

var dataRepresentation: Data?

Returns the PDF data (that is, a PDF document) representing this page. This method does not preserve external page links.

var pageRef: CGPDFPage?

### Instance Methods

func draw(with: PDFDisplayBox, to: CGContext)

func thumbnail(of: CGSize, for: PDFDisplayBox) -> UIImage

func transform(CGContext, for: PDFDisplayBox)

func transform(for: PDFDisplayBox) -> CGAffineTransform

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

class PDFOutline

A `PDFOutline` object is an element in a tree-structured hierarchy that can represent the structure of a PDF document.

class PDFSelection

A `PDFSelection` object identifies a contiguous or noncontiguous selection of text in a PDF document.

