

- UIKit
- UIToolbar
-  shadowImage(forToolbarPosition:) 

Instance Method

# shadowImage(forToolbarPosition:)

Returns the image to use for the toolbar shadow in a given position.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func shadowImage(forToolbarPosition topOrBottom: UIBarPosition) -> UIImage?
```

## Parameters 

`topOrBottom`  

A toolbar position constant. You can use this parameter to indicate whether the shadow image returned is intended for use in a toolbar at the top or bottom of the view.

## Return Value

The image to use for the toolbar shadow in the position specified by `topOrBottom`.

## Discussion

The default value is `nil`, which corresponds to the default shadow image being used. When non-`nil`, the return value represents the shadow that is used on the toolbar in the position specified by the `topOrBottom` parameter.

## See Also

### Adding a shadow

func setShadowImage(UIImage?, forToolbarPosition: UIBarPosition)

Sets the image to use for the toolbar shadow in a given position.

