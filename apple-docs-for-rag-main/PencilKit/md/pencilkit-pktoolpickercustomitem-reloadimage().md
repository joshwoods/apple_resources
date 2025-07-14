

- PencilKit
- PKToolPickerCustomItem
-  reloadImage() 

Instance Method

# reloadImage()

Requests a new image for the custom tool item from the image provider.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
func reloadImage()
```

## Discussion

Calling this method requests a new image for the custom tool item from the imageProvider of the configuration.

The system automatically calls this method when PencilKit attributes like color or width change. You can call this method when you need to generate a new image for the custom tool item that’s different from the current image.

