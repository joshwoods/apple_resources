

- Quartz
- IKImageEditPanelDataSource
-  image 

Instance Property

# image

Returns an image.

macOS 10.4+

``` source
var image: CGImage! { get }
```

**Required**

## Return Value

An image.

## Discussion

Your data source must implement this method.

## See Also

### Getting Images From the Data Source

func thumbnail(withMaximumSize: NSSize) -> Unmanaged&lt;CGImage>!

Returns a thumbnail image whose size is no larger than the specified size.

