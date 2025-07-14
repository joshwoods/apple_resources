

- PDFKit
- PDFView
-  Configurations 

API Collection

# Configurations

Define display modes, scaling, rendering, printing and graphics properties.

## Topics

### Working with Display Modes and Characteristics

var displayMode: PDFDisplayMode

The current display mode.

enum PDFDisplayMode

A wrapper for the chosen display mode constant.

Additional Display Configurations

Operations for setting up page breaks, a display box, and display direction.

Book Display

Operations to setup a book display for a PDF view.

Graphics Properties

Operations to define the background color, antialiasing, and greeking for a PDF view.

### Scaling the View

var scaleFactor: CGFloat

The current scale factor for the view.

var scaleFactorForSizeToFit: CGFloat

The “size to fit” scale factor that `autoScales` would use for scaling the current document and layout.

var maxScaleFactor: CGFloat

The maximum scaling factor for the PDF document.

var minScaleFactor: CGFloat

The minimum scaling factor for the PDF document.

var autoScales: Bool

A Boolean value indicating whether autoscaling is set.

func rowSize(for: PDFPage) -> CGSize

Returns the size needed to display a row of the current document page.

Zoom Operations

Zoom operations for a PDF View.

### Rendering the View and Printing

func draw(PDFPage)

Draw and render a visible page.

Deprecated

func drawPagePost(PDFPage)

Perform post-page rendering.

Deprecated

func print(with: NSPrintInfo, autoRotate: Bool)

Prints the document with the specified printer information.

func print(with: NSPrintInfo, autoRotate: Bool, pageScaling: PDFPrintScalingMode)

Prints the document with the specified printer and page-scaling information.

### Specializing the View

var documentView: UIView?

The innermost view used by `PDFView` or by your `PDFView` subclass.

func layoutDocumentView()

Performs layout of the inner views.

Draw Operations

Draw in a PDF page.

