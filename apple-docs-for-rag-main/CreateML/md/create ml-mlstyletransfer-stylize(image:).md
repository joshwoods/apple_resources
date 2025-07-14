

- Create ML
- MLStyleTransfer
-  stylize(image:) 

Instance Method

# stylize(image:)

Applies the style the model learned to an image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
func stylize(image: CGImage) throws -> CGImage?
```

## Parameters 

`image`  

An input image the model applies its style to.

## Return Value

An image of type `CGImage` stylized using style of the model.

## Discussion

Throws

`MLCreateError.generic` if stylization fails.

