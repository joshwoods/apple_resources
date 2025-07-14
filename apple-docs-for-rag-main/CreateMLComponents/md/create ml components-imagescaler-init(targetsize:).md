

- Create ML Components
- ImageScaler
-  init(targetSize:) 

Initializer

# init(targetSize:)

Creates an image scaler transformer. This transformer is used to scale an image to the `targetSize`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(targetSize: CGSize)
```

## Parameters 

`targetSize`  

The target image size. Both width and height must be positive.

## See Also

### Creating a transformer

init(targetHeight: Double)

Creates an image scaler transformer that preserves the aspect ratio.

init(targetWidth: Double)

Creates an image scaler transformer that preserves the aspect ratio.

