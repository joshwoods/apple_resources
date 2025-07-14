

- UIKit
- UIImage
-  stretchableImage(withLeftCapWidth:topCapHeight:) Deprecated

Instance Method

# stretchableImage(withLeftCapWidth:topCapHeight:)

Creates and returns a new image object with the specified cap values.

iOSiPadOSMac CatalystvisionOSwatchOS

``` source
func stretchableImage(
    withLeftCapWidth leftCapWidth: Int,
    topCapHeight: Int
) -> UIImage
```

Deprecated

Use the resizableImage(withCapInsets:) instead, specifying cap insets such that the interior is a `1x1` area.

## Parameters 

`leftCapWidth`  

The value to use for the left cap width. Specify `0` if you want the entire image to be horizontally stretchable. For a discussion of how a non-zero value affects the image, see the leftCapWidth property.

`topCapHeight`  

The value to use for the top cap height. Specify `0` if you want the entire image to be vertically stretchable. For a discussion of how a non-zero value affects the image, see the topCapHeight property.

## Return Value

A new image object with the specified cap values.

## Discussion

During scaling or resizing of the image, areas covered by a cap are not scaled or resized. Instead, the 1-pixel wide area not covered by the cap in each direction is what is scaled or resized. This technique is often used to create variable-width buttons, which retain the same rounded corners but whose center region grows or shrinks as needed.

You use this method to add cap values to an image or to change the existing cap values of an image. In both cases, you get back a new image and the original image remains untouched.

## See Also

### Deprecated

var leftCapWidth: Int

The horizontal end-cap size.

Deprecated

var topCapHeight: Int

The vertical end-cap size.

Deprecated

