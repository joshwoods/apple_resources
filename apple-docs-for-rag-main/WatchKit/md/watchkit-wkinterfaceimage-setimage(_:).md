

- WatchKit
- WKInterfaceImage
-  setImage(\_:) 

Instance Method

# setImage(\_:)

Sets the displayed image using the specified image object.

watchOS 2.0+

``` source
func setImage(_ image: UIImage?)
```

## Parameters 

`image`  

The image to be displayed. Specifying `nil` removes the existing image, causing the watch interface to display nothing in the space previously occupied by the image. You may specify a template image or an animated image sequence for this parameter. For information on how to specify an animated image, see Animating a Series of Images.

## Discussion

This method changes the image being displayed. Use this method to assign either a static image or an animated image that you created using the animatedImage(with:duration:) method.

When setting images, always try to use images that are sized to fit the available space. Images are rendered according to the mode and size attributes you set for the image interface object.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Configuring the Image

func setImageData(Data?)

Sets the displayed image using a formatted data object.

func setImageNamed(String?)

Sets the displayed image using a named image resource file.

func setTintColor(UIColor?)

Changes the color applied to a template image.

