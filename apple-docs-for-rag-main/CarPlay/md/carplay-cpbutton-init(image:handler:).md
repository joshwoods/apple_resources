

- CarPlay
- CPButton
-  init(image:handler:) 

Initializer

# init(image:handler:)

Creates a button that displays an image and invokes a handler when the user taps it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    image: UIImage,
    handler: ((CPButton) -> Void)? = nil
)
```

## Parameters 

`image`  

The image that the button displays.

`handler`  

The closure that the button invokes when the user taps it.

## Return Value

A new button that displays an image and invokes its handler when the user taps it.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property, and ensure it is no larger than CPButtonMaximumImageSize.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

## See Also

### Creating a Button

let CPButtonMaximumImageSize: CGSize

The maximum size of a button’s image that CarPlay supports.

