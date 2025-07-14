

- Quartz
- IKImageEditPanelDataSource
-  setImage(\_:imageProperties:) 

Instance Method

# setImage(\_:imageProperties:)

Sets an image with the specified properties.

macOS 10.4+

``` source
func setImage(
    _ image: CGImage!,
    imageProperties metaData: [AnyHashable : Any]!
)
```

**Required**

## Discussion

Your data source must implement this method.

## See Also

### Related Documentation

protocol IKImageEditPanelDataSource

The `IKImageEditPanelDataSource` protocol describes the methods that an IKImageEditPanel object uses to access the contents of its data source object.

### Getting and Setting Image Properties

var imageProperties: [AnyHashable : Any]!

Returns a dictionary of the image properties associated with the image in the image edit panel.

