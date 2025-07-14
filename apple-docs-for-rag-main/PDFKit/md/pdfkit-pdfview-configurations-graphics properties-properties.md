

- PDFKit
- PDFView
- Configurations
-  Graphics Properties 

API Collection

# Graphics Properties

Operations to define the background color, antialiasing, and greeking for a PDF view.

## Topics

### Setting Background Color

func takeBackgroundColorFrom(Any)

Sets the view’s background color to the specified color.

Deprecated

var backgroundColor: UIColor

The view’s background color.

### Antialiasing

var shouldAntiAlias: Bool

A Boolean value indicating whether the view is antialiased.

Deprecated

var interpolationQuality: PDFInterpolationQuality

The interpolation quality for images drawn into the `PDFView` context.

enum PDFInterpolationQuality

A wrapper for the specified interpolation quality.

### Greeking

var greekingThreshold: CGFloat

Returns the current greeking threshold for the view.

Deprecated

## See Also

### Working with Display Modes and Characteristics

var displayMode: PDFDisplayMode

The current display mode.

enum PDFDisplayMode

A wrapper for the chosen display mode constant.

Additional Display Configurations

Operations for setting up page breaks, a display box, and display direction.

Book Display

Operations to setup a book display for a PDF view.

