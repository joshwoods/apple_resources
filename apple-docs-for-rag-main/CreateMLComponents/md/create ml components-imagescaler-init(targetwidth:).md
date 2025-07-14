

- Create ML Components
- ImageScaler
-  init(targetWidth:) 

Initializer

# init(targetWidth:)

Creates an image scaler transformer that preserves the aspect ratio.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(targetWidth: Double)
```

## Parameters 

`targetWidth`  

The target image width. It must be positive.

## Discussion

This transformer scales an image to match the `targetWidth` while preserving the aspect ratio.

## See Also

### Creating a transformer

init(targetSize: CGSize)

Creates an image scaler transformer. This transformer is used to scale an image to the `targetSize`.

init(targetHeight: Double)

Creates an image scaler transformer that preserves the aspect ratio.

