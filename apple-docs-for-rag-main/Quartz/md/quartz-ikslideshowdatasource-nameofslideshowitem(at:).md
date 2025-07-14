

- Quartz
- IKSlideshowDataSource
-  nameOfSlideshowItem(at:) 

Instance Method

# nameOfSlideshowItem(at:)

Returns the display name for item at the specified index.

macOS 10.4+

``` source
optional func nameOfSlideshowItem(at index: Int) -> String!
```

## Parameters 

`index`  

The index for a slideshow item.

## Return Value

The display name. For the best user experience, you should provide the localized name, because this string appears in the user interface.

## Discussion

This method is optional.

## See Also

### Providing Slideshow Information

func numberOfSlideshowItems() -> Int

Returns the number of items in a slideshow.

**Required**

func slideshowItem(at: Int) -> Any!

Returns the item for a given index

**Required**

func canExportSlideshowItem(at: Int, toApplication: String!) -> Bool

Reports whether the export button should be enabled for a slideshow item.

