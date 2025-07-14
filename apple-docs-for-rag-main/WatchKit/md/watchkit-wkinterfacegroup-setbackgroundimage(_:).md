

- WatchKit
- WKInterfaceGroup
-  setBackgroundImage(\_:) 

Instance Method

# setBackgroundImage(\_:)

Changes the background image of the group container to the specified image.

watchOS 2.0+

``` source
func setBackgroundImage(_ image: UIImage?)
```

## Parameters 

`image`  

The background image to be displayed behind all items in the group. Specifying `nil` removes the existing image, causing the background color to show through. You may specify an image object that contains multiple images running as an animation.

## See Also

### Setting the Group’s Content

func setBackgroundColor(UIColor?)

Changes the background color for the group container.

func setBackgroundImageData(Data?)

Changes the background image of the group container to the image in the specified data object.

func setBackgroundImageNamed(String?)

Changes the background image of the group container to the image in the specified resource file.

