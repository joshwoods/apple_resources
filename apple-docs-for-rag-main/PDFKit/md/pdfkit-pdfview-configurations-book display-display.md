

- PDFKit
- PDFView
- Configurations
-  Book Display 

API Collection

# Book Display

Operations to setup a book display for a PDF view.

## Topics

### Displaying as Book

var displaysAsBook: Bool

A Boolean value indicating whether the view will display the first page as a book cover (meaningful only when the document is in two-up or two-up continuous display mode).

var isUsingPageViewController: Bool

A Boolean value indicating whether the scroll view is using a `UIPageViewController`.

func usePageViewController(Bool, withViewOptions: [AnyHashable : Any]?)

Changes the scroll view to use a `UIPageViewController` to layout and navigate pages.

## See Also

### Working with Display Modes and Characteristics

var displayMode: PDFDisplayMode

The current display mode.

enum PDFDisplayMode

A wrapper for the chosen display mode constant.

Additional Display Configurations

Operations for setting up page breaks, a display box, and display direction.

Graphics Properties

Operations to define the background color, antialiasing, and greeking for a PDF view.

