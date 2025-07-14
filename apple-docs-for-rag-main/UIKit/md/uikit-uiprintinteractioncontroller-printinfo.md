

- UIKit
- UIPrintInteractionController
-  printInfo 

Instance Property

# printInfo

An object that encapsulates information about the print job.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printInfo: UIPrintInfo? { get set }
```

## Discussion

An instance of UIPrintInfo includes properties such as the print-job name, the printer identifier, the orientation of the printed content, the duplex mode, and the kind of content (general, photo, or grayscale). If you do not assign an instance of UIPrintInfo to this property, the UIKit printing system assumes defaults for many of these properties. Users can modify the selected printer and the duplex mode (if available on the printer). Once the printing options are presented, any changes to the `UIPrintInfo` object referenced by this property are ignored. The object is released when printing completes.

## See Also

### Accessing print-job information

var printPaper: UIPrintPaper?

An object that represents the paper size and printing area for the print job.

var showsNumberOfCopies: Bool

A Boolean value that determines whether the printing options include the number of copies.

var showsPaperSelectionForLoadedPapers: Bool

A Boolean value that determines whether the paper selection menu displays.

var showsPaperOrientation: Bool

A Boolean value that indicates whether the printing options include the paper-orientation control.

var showsPageRange: Bool

A Boolean value that determines whether the printing options include a page-range control.

Deprecated

