

- Media Player
- MPMediaItemArtwork
-  init(image:) Deprecated

Initializer

# init(image:)

Initializes a media item artwork instance with a full-size image.

iOS 5.0–10.0DeprecatediPadOS 5.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
convenience init(image: UIImage)
```

Deprecated

Use -initWithBoundsSize:requestHandler:

## Parameters 

`image`  

The image to use to initialize the media item artwork instance.

## Discussion

This method assumes that the crop rectangle of the image matches the bounds of the image, as defined by the image’s size in points. That is, this method assumes the image you supply is tightly cropped.

