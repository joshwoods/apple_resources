

- Quartz
- IKSlideshowDataSource
-  numberOfSlideshowItems() 

Instance Method

# numberOfSlideshowItems()

Returns the number of items in a slideshow.

macOS 10.4+

``` source
func numberOfSlideshowItems() -> Int
```

**Required**

## Return Value

The number of items in the slideshow.

## Discussion

Your data source must implement this method.

## See Also

### Providing Slideshow Information

func slideshowItem(at: Int) -> Any!

Returns the item for a given index

**Required**

func nameOfSlideshowItem(at: Int) -> String!

Returns the display name for item at the specified index.

func canExportSlideshowItem(at: Int, toApplication: String!) -> Bool

Reports whether the export button should be enabled for a slideshow item.

