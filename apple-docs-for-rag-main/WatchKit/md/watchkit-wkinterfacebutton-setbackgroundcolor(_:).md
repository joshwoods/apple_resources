

- WatchKit
- WKInterfaceButton
-  setBackgroundColor(\_:) 

Instance Method

# setBackgroundColor(\_:)

Sets the background color of the button.

watchOS 2.0+

``` source
func setBackgroundColor(_ color: UIColor?)
```

## Parameters 

`color`  

The fill color to use for the button’s background.

## Discussion

If you specify both a background color and a full-color background image, only the image is displayed. If the image is a template image instead, the button tints the image using the background color.

## See Also

### Setting the Button Background

func setBackgroundImage(UIImage?)

Sets the button’s background image to the specified image.

func setBackgroundImageData(Data?)

Sets the button’s background image to the image in the specified data object.

func setBackgroundImageNamed(String?)

Sets the button’s background image to the image in the named resource file.

