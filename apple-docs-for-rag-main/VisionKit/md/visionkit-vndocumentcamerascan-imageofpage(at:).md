

- VisionKit
- VNDocumentCameraScan
-  imageOfPage(at:) 

Instance Method

# imageOfPage(at:)

Requests the image of a page at a specified index.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func imageOfPage(at index: Int) -> UIImage
```

## Parameters 

`index`  

The index of the image in the scanned document you’d like to return. Page 1 is at index 0.

## Return Value

The image of the page at the specified index. If `index` is out of bounds, the framework throws an exception.

## See Also

### Reading the scanned document

var title: String

The title of the scanned document.

var pageCount: Int

The number of pages in the scanned document.

