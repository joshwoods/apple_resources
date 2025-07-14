

- PDFKit
- PDFPage
-  document 

Instance Property

# document

Returns the `PDFDocument` object with which the page is associated.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
weak var document: PDFDocument? { get }
```

## See Also

### Getting Information About a Page

var label: String?

Returns the label for the page.

func bounds(for: PDFDisplayBox) -> CGRect

Returns the bounds for the specified PDF display box.

func setBounds(CGRect, for: PDFDisplayBox)

Sets the bounds for the specified box.

var rotation: Int

Sets the rotation angle for the page in degrees.

