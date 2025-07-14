

- Quartz
- IKSlideshowDataSource
-  slideshowItem(at:) 

Instance Method

# slideshowItem(at:)

Returns the item for a given index

macOS 10.4+

``` source
func slideshowItem(at index: Int) -> Any!
```

**Required**

## Parameters 

`index`  

An index of an item in the slideshow.

## Return Value

The object that corresponds to the item at the specified index. The item can be any of the following objects: NSImage, NSString (to specify a path name), NSURL, FileWrapper, CGImage, or PDFPage.

## Discussion

Your data source must implement this method.

## See Also

### Providing Slideshow Information

func numberOfSlideshowItems() -> Int

Returns the number of items in a slideshow.

**Required**

func nameOfSlideshowItem(at: Int) -> String!

Returns the display name for item at the specified index.

func canExportSlideshowItem(at: Int, toApplication: String!) -> Bool

Reports whether the export button should be enabled for a slideshow item.

