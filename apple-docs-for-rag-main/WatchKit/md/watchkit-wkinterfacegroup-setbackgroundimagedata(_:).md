

- WatchKit
- WKInterfaceGroup
-  setBackgroundImageData(\_:) 

Instance Method

# setBackgroundImageData(\_:)

Changes the background image of the group container to the image in the specified data object.

watchOS 2.0+

``` source
func setBackgroundImageData(_ imageData: Data?)
```

## Parameters 

`imageData`  

A data object containing the image data in its native format. Specifying `nil` removes the existing image, causing the watch interface to display nothing in the space previously occupied by the image.

## Discussion

Use this method when you already have image data in the raw PNG or JPG format. This method sends the data as-is, which lets you send the data in a compressed format. Sending compressed data is often more efficient than sending a UIImage object.

## See Also

### Setting the Group’s Content

func setBackgroundColor(UIColor?)

Changes the background color for the group container.

func setBackgroundImage(UIImage?)

Changes the background image of the group container to the specified image.

func setBackgroundImageNamed(String?)

Changes the background image of the group container to the image in the specified resource file.

