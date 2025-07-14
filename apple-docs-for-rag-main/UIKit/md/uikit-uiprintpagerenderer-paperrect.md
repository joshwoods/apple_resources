

- UIKit
- UIPrintPageRenderer
-  paperRect 

Instance Property

# paperRect

The size of the paper for printing.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var paperRect: CGRect { get }
```

## Discussion

The value of this property is a rectangle that defines the size of paper chosen for the print job. The origin is always (0,0).

## See Also

### Related Documentation

var printPaper: UIPrintPaper?

An object that represents the paper size and printing area for the print job.

### Accessing information about the print job

var numberOfPages: Int

The number of pages to render.

var printableRect: CGRect

The area in which printing can occur.

