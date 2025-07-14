

- UIKit
- UIPrintInteractionController
-  showsPaperSelectionForLoadedPapers 

Instance Property

# showsPaperSelectionForLoadedPapers

A Boolean value that determines whether the paper selection menu displays.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var showsPaperSelectionForLoadedPapers: Bool { get set }
```

## Discussion

The default value of this property is false. Setting the value to true enables a paper selection menu on printers that support different types of paper and have more than one paper type loaded. On printers where only one paper type is available, no paper selection menu is displayed, regardless of the value of this property.

## See Also

### Accessing print-job information

var printInfo: UIPrintInfo?

An object that encapsulates information about the print job.

var printPaper: UIPrintPaper?

An object that represents the paper size and printing area for the print job.

var showsNumberOfCopies: Bool

A Boolean value that determines whether the printing options include the number of copies.

var showsPaperOrientation: Bool

A Boolean value that indicates whether the printing options include the paper-orientation control.

var showsPageRange: Bool

A Boolean value that determines whether the printing options include a page-range control.

Deprecated

