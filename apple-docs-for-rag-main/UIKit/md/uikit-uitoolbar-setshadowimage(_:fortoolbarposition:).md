

- UIKit
- UIToolbar
-  setShadowImage(\_:forToolbarPosition:) 

Instance Method

# setShadowImage(\_:forToolbarPosition:)

Sets the image to use for the toolbar shadow in a given position.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setShadowImage(
    _ shadowImage: UIImage?,
    forToolbarPosition topOrBottom: UIBarPosition
)
```

## Parameters 

`shadowImage`  

The image to use for the toolbar shadow in the position specified by `topOrBottom`.

`topOrBottom`  

A toolbar position constant. You can use this parameter to indicate whether the `shadowImage` is intended for a toolbar at the top or bottom of the view.

## Discussion

When the `shadowImage` parameter is `nil`, the default shadow will be used. When non-`nil`, the `shadowImage` property is a custom shadow image to show instead of the default. Using the `topOrBottom` parameter, you can set a different shadow for toolbars at the top and bottom of the view. For a custom shadow image to be shown, a custom background image must also be set with the setBackgroundImage(_:forToolbarPosition:barMetrics:) method. If the default background image is used, then the default shadow image will be used regardless of the value of the `shadowImage` parameter.

## See Also

### Adding a shadow

func shadowImage(forToolbarPosition: UIBarPosition) -> UIImage?

Returns the image to use for the toolbar shadow in a given position.

