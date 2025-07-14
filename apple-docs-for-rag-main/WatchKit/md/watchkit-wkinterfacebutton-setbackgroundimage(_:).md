

- WatchKit
- WKInterfaceButton
-  setBackgroundImage(\_:) 

Instance Method

# setBackgroundImage(\_:)

Sets the button’s background image to the specified image.

watchOS 2.0+

``` source
func setBackgroundImage(_ image: UIImage?)
```

## Parameters 

`image`  

The image to be displayed behind the button’s title text. The image is displayed behind the button’s title text. Specifying `nil` removes the existing image. You may specify an image object that contains multiple images running as an animation. The image is scaled as needed to fill the button’s content area.

## Discussion

If `image` is a template image, the button tints that image using the current background color. The button does not use the background color for full-color images.

## See Also

### Setting the Button Background

func setBackgroundColor(UIColor?)

Sets the background color of the button.

func setBackgroundImageData(Data?)

Sets the button’s background image to the image in the specified data object.

func setBackgroundImageNamed(String?)

Sets the button’s background image to the image in the named resource file.

