

- WatchKit
- WKInterfaceButton
-  setBackgroundImageData(\_:) 

Instance Method

# setBackgroundImageData(\_:)

Sets the button’s background image to the image in the specified data object.

watchOS 2.0+

``` source
func setBackgroundImageData(_ imageData: Data?)
```

## Parameters 

`imageData`  

A data object containing the image data in its native format. The image is displayed behind the button’s title text. Specifying `nil` removes the existing image. You may specify image data that contains multiple images running as an animation. The image is scaled as needed to fill the button’s content area.

## Discussion

Use this method when you already have image data in the raw PNG or JPG format. This method sends the data as-is, which lets you send the data in a compressed format. Sending compressed data is often more efficient than sending a UIImage object.

## See Also

### Setting the Button Background

func setBackgroundColor(UIColor?)

Sets the background color of the button.

func setBackgroundImage(UIImage?)

Sets the button’s background image to the specified image.

func setBackgroundImageNamed(String?)

Sets the button’s background image to the image in the named resource file.

