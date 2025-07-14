

- Quartz
- IKImageEditPanelDataSource
-  imageProperties 

Instance Property

# imageProperties

Returns a dictionary of the image properties associated with the image in the image edit panel.

macOS 10.4+

``` source
optional var imageProperties: [AnyHashable : Any]! { get }
```

## Return Value

A dictionary that contains the properties of the image.

## See Also

### Related Documentation

protocol IKImageEditPanelDataSource

The `IKImageEditPanelDataSource` protocol describes the methods that an IKImageEditPanel object uses to access the contents of its data source object.

Image Kit Programming Guide

### Getting and Setting Image Properties

func setImage(CGImage!, imageProperties: [AnyHashable : Any]!)

Sets an image with the specified properties.

**Required**

