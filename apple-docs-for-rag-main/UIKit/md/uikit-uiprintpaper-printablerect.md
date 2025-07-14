

- UIKit
- UIPrintPaper
-  printableRect 

Instance Property

# printableRect

The rectangle that represents the portion of the paper that can be imaged upon.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printableRect: CGRect { get }
```

## Discussion

Typically, UIKit passes this value into the last argument of the UIPrintPageRenderer method drawPage(at:in:).

## See Also

### Getting the paper size and the printing area

var paperSize: CGSize

The size of the sheet to use for printing.

