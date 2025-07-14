

- UIKit
- UIPrintInteractionController
-  printPaper 

Instance Property

# printPaper

An object that represents the paper size and printing area for the print job.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printPaper: UIPrintPaper? { get }
```

## Discussion

`UIPrintInteractionController` sets this property immediately after the user selects a printer and before it calls the delegate’s printInteractionControllerWillStartJob(_:) method. If its delegate implements the printInteractionController(_:choosePaper:) method of the `UIPrintInteractionControllerDelegate` protocol, it can return the UIPrintPaper object to assign to this property. Otherwise, UIKit assigns an object with a default paper size and printing rectangle that is based on the output type and the capabilities of the destination printer. This object is released when the print job finishes.

## See Also

### Accessing print-job information

var printInfo: UIPrintInfo?

An object that encapsulates information about the print job.

var showsNumberOfCopies: Bool

A Boolean value that determines whether the printing options include the number of copies.

var showsPaperSelectionForLoadedPapers: Bool

A Boolean value that determines whether the paper selection menu displays.

var showsPaperOrientation: Bool

A Boolean value that indicates whether the printing options include the paper-orientation control.

var showsPageRange: Bool

A Boolean value that determines whether the printing options include a page-range control.

Deprecated

