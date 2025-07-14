

- UIKit
- UIPrintPaper
-  paperSize 

Instance Property

# paperSize

The size of the sheet to use for printing.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var paperSize: CGSize { get }
```

## Discussion

The paper size is often associated with a standard designation, such as “Letter” and “A4”. For example, the paper size for a Letter sheet of paper is 612 points wide and 792 points high.

## See Also

### Getting the paper size and the printing area

var printableRect: CGRect

The rectangle that represents the portion of the paper that can be imaged upon.

