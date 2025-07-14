

- WatchKit
- WKInterfaceButton
-  setBackgroundImageNamed(\_:) 

Instance Method

# setBackgroundImageNamed(\_:)

Sets the button’s background image to the image in the named resource file.

watchOS 2.0+

``` source
func setBackgroundImageNamed(_ imageName: String?)
```

## Parameters 

`imageName`  

The name of the image to load from the Watch app’s bundle. For images in the bundle, specify the filename of the image and include the filename extension in the name. The image is displayed behind the button’s title text. You may specify an image file that contains multiple images running as an animation. The image is scaled as needed to fill the button’s content area.

## Discussion

This method looks for an image with the specified name in the Watch app’s bundle and uses it as the background image for the button. (In watchOS 1, the button also searches the image cache for an image with the specified name.) If the specified image cannot be found, the button displays no background image.

When the image is a template image, the button tints that image using the current background color. The button does not use the background color for full-color images.

## See Also

### Setting the Button Background

func setBackgroundColor(UIColor?)

Sets the background color of the button.

func setBackgroundImage(UIImage?)

Sets the button’s background image to the specified image.

func setBackgroundImageData(Data?)

Sets the button’s background image to the image in the specified data object.

