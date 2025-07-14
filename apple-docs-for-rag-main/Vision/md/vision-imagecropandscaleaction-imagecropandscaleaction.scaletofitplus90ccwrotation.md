

- Vision
- ImageCropAndScaleAction
-  ImageCropAndScaleAction.scaleToFitPlus90CCWRotation 

Case

# ImageCropAndScaleAction.scaleToFitPlus90CCWRotation

An action that scales the image and maintains the aspect ratio to fit on the long side, and rotates the image by 90 degrees counter clockwise.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
case scaleToFitPlus90CCWRotation
```

## Discussion

Rotation helps to optimize portrait images fit into landscape buffers for algorithms that are rotation agnostic.

## See Also

### Getting the actions

case centerCrop

An action that scales the image and maintains the aspect ratio to fit on the short side and crop centered on the long side.

case scaleToFit

An action that scales to the size the algorithm requires while maintaining the original aspect ratio.

case scaleToFill

An action that scales the image to fill the input dimensions and resizing it, if necessary.

case scaleToFillPlus90CCWRotation

An action that scales the image and rotates it by 90 degrees counter clockwise.

