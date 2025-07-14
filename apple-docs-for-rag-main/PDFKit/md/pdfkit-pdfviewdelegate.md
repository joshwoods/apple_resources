

- PDFKit
-  PDFViewDelegate 

Protocol

# PDFViewDelegate

The delegate for the `PDFView` object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
protocol PDFViewDelegate : NSObjectProtocol
```

## Topics

### Working with Annotation Actions

func pdfViewPerformFind(PDFView)

Performs a find operation.

func pdfViewPerformGo(toPage: PDFView)

Performs a go-to operation.

func pdfViewPerformPrint(PDFView)

Prints the current document.

func pdfViewOpenPDF(PDFView, forRemoteGoToAction: PDFActionRemoteGoTo)

Opens a specified page.

### Scaling the View

func pdfViewWillChangeScaleFactor(PDFView, toScale: CGFloat) -> CGFloat

Overrides changes to the scale factor.

### Linking in a View

func pdfViewWillClick(onLink: PDFView, with: URL)

Handle clicks on URL links in a view.

### Printing the View

func pdfViewPrintJobTitle(PDFView) -> String

Overrides the job title used when the `PDFView` is printed.

### Instance Methods

func pdfViewParentViewController() -> UIViewController

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the Delegate

var delegate: (any PDFViewDelegate)?

Returns the view’s delegate.

