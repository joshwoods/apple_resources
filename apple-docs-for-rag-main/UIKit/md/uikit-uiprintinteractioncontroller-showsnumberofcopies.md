

- UIKit
- UIPrintInteractionController
-  showsNumberOfCopies 

Instance Property

# showsNumberOfCopies

A Boolean value that determines whether the printing options include the number of copies.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var showsNumberOfCopies: Bool { get set }
```

## Discussion

The default value is true.

## See Also

### Accessing print-job information

var printInfo: UIPrintInfo?

An object that encapsulates information about the print job.

var printPaper: UIPrintPaper?

An object that represents the paper size and printing area for the print job.

var showsPaperSelectionForLoadedPapers: Bool

A Boolean value that determines whether the paper selection menu displays.

var showsPaperOrientation: Bool

A Boolean value that indicates whether the printing options include the paper-orientation control.

var showsPageRange: Bool

A Boolean value that determines whether the printing options include a page-range control.

Deprecated

