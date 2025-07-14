

- CarPlay
- CPContact
-  init(name:image:) 

Initializer

# init(name:image:)

Creates a contact with a name and an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    name: String,
    image: UIImage
)
```

## Parameters 

`name`  

The name that the template displays.

`image`  

The image that the template displays beside the contact’s name.

## Return Value

A new contact with the provided name and image.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

