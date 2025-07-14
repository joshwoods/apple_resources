

- VisionKit
- VNDocumentCameraScan
-  pageCount 

Instance Property

# pageCount

The number of pages in the scanned document.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var pageCount: Int { get }
```

## See Also

### Reading the scanned document

var title: String

The title of the scanned document.

func imageOfPage(at: Int) -> UIImage

Requests the image of a page at a specified index.

