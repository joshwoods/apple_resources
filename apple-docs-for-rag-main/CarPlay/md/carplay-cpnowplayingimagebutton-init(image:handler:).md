

- CarPlay
- CPNowPlayingImageButton
-  init(image:handler:) 

Initializer

# init(image:handler:)

Creates a Now Playing button that displays a custom image and invokes a handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    image: UIImage,
    handler: ((CPNowPlayingButton) -> Void)? = nil
)
```

## Parameters 

`image`  

An image to display on the button.

`handler`  

A closure that the button invokes when the user taps it.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen—see your interface controller’s carTraitCollection property—and make sure it is no larger than CPNowPlayingButtonMaximumImageSize.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

## See Also

### Creating a Button

let CPNowPlayingButtonMaximumImageSize: CGSize

The maximum size CarPlay supports for a button’s image.

