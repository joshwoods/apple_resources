

- WatchKit
- WKInterfaceGroup
-  setBackgroundImageNamed(\_:) 

Instance Method

# setBackgroundImageNamed(\_:)

Changes the background image of the group container to the image in the specified resource file.

watchOS 2.0+

``` source
func setBackgroundImageNamed(_ imageName: String?)
```

## Parameters 

`imageName`  

The name of the image to be loaded from the WatchKit app’s bundle. For images in the bundle, specify the filename of the image and include the filename extension in the name. You may specify an image file that contains multiple images running as an animation.

## Discussion

This method looks for an image with the specified name in the Watch app’s bundle and uses it as the background image for the group. If the specified image cannot be found, the group displays no background image.

## See Also

### Setting the Group’s Content

func setBackgroundColor(UIColor?)

Changes the background color for the group container.

func setBackgroundImage(UIImage?)

Changes the background image of the group container to the specified image.

func setBackgroundImageData(Data?)

Changes the background image of the group container to the image in the specified data object.

