

- WatchKit
- WKInterfaceImage
-  setImageData(\_:) 

Instance Method

# setImageData(\_:)

Sets the displayed image using a formatted data object.

watchOS 2.0+

``` source
func setImageData(_ imageData: Data?)
```

## Parameters 

`imageData`  

A data object containing the image data in its native format. Specifying `nil` removes the existing image, causing the watch interface to display nothing in the space previously occupied by the image.

## Discussion

This method changes the image being displayed.

When setting images, always try to use images that are sized to fit the available space. Images are rendered according to the mode and size attributes you set for the image interface object.

## See Also

### Configuring the Image

func setImage(UIImage?)

Sets the displayed image using the specified image object.

func setImageNamed(String?)

Sets the displayed image using a named image resource file.

func setTintColor(UIColor?)

Changes the color applied to a template image.

