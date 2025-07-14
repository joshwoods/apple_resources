

- UIKit
- UIPrintInteractionController
-  showsPageRange Deprecated

Instance Property

# showsPageRange

A Boolean value that determines whether the printing options include a page-range control.

iOS 4.2–10.0DeprecatediPadOS 4.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var showsPageRange: Bool { get set }
```

## Discussion

The default value is false. If you assign printable content to the printingItems property, the page-range control is not shown, even if `showPageRange` is true. In other cases, the number of pages to print must be greater than 1 form the page-range control to appear.

## See Also

### Accessing print-job information

var printInfo: UIPrintInfo?

An object that encapsulates information about the print job.

var printPaper: UIPrintPaper?

An object that represents the paper size and printing area for the print job.

var showsNumberOfCopies: Bool

A Boolean value that determines whether the printing options include the number of copies.

var showsPaperSelectionForLoadedPapers: Bool

A Boolean value that determines whether the paper selection menu displays.

var showsPaperOrientation: Bool

A Boolean value that indicates whether the printing options include the paper-orientation control.

