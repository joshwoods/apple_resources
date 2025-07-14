

- Quartz
- IKSlideshowDataSource
-  canExportSlideshowItem(at:toApplication:) 

Instance Method

# canExportSlideshowItem(at:toApplication:)

Reports whether the export button should be enabled for a slideshow item.

macOS 10.4+

``` source
optional func canExportSlideshowItem(
    at index: Int,
    toApplication applicationBundleIdentifier: String!
) -> Bool
```

## Return Value

true if the export button should be enabled for an item; otherwise false.

## See Also

### Providing Slideshow Information

func numberOfSlideshowItems() -> Int

Returns the number of items in a slideshow.

**Required**

func slideshowItem(at: Int) -> Any!

Returns the item for a given index

**Required**

func nameOfSlideshowItem(at: Int) -> String!

Returns the display name for item at the specified index.

