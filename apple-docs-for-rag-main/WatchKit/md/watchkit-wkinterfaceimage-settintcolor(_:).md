

- WatchKit
- WKInterfaceImage
-  setTintColor(\_:) 

Instance Method

# setTintColor(\_:)

Changes the color applied to a template image.

watchOS 2.0+

``` source
func setTintColor(_ tintColor: UIColor?)
```

## Parameters 

`tintColor`  

The tint color to use for a template image. Specify `nil` to use the default tint color.

## Discussion

When you display a template image, use this method to set the tint color to apply to that image. With a template image, WatchKit uses only the alpha channel of the image to define a shape. To create a template image from an existing image, call the withRenderingMode(_:) method on an existing UIImage and specify the UIImage.RenderingMode.alwaysTemplate rendering mode.

An image object applies the tint color only when it contains a single template image. It does not apply the tint color to animated images or images that are not configured as template images.

## See Also

### Configuring the Image

func setImage(UIImage?)

Sets the displayed image using the specified image object.

func setImageData(Data?)

Sets the displayed image using a formatted data object.

func setImageNamed(String?)

Sets the displayed image using a named image resource file.

