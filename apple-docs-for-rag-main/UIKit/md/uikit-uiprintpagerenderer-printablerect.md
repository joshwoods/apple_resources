

- UIKit
- UIPrintPageRenderer
-  printableRect 

Instance Property

# printableRect

The area in which printing can occur.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printableRect: CGRect { get }
```

## Discussion

The value of this property is a rectangle that defines the area in which the printer can print content. Sometimes this is referred to as the imageable area of the paper.

## See Also

### Related Documentation

var printPaper: UIPrintPaper?

An object that represents the paper size and printing area for the print job.

### Accessing information about the print job

var numberOfPages: Int

The number of pages to render.

var paperRect: CGRect

The size of the paper for printing.

