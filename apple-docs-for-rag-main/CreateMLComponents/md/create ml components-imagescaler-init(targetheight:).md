

- Create ML Components
- ImageScaler
-  init(targetHeight:) 

Initializer

# init(targetHeight:)

Creates an image scaler transformer that preserves the aspect ratio.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(targetHeight: Double)
```

## Parameters 

`targetHeight`  

The target image height. It must be positive.

## Discussion

This transformer scales an image to match the `targetHeight` while preserving the aspect ratio.

## See Also

### Creating a transformer

init(targetSize: CGSize)

Creates an image scaler transformer. This transformer is used to scale an image to the `targetSize`.

init(targetWidth: Double)

Creates an image scaler transformer that preserves the aspect ratio.

