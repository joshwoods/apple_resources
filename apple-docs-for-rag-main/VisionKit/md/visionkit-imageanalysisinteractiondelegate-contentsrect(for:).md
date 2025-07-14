

- VisionKit
- ImageAnalysisInteractionDelegate
-  contentsRect(for:) 

Instance Method

# contentsRect(for:)

Returns the rectangle, in unit coordinates, that contains the image within the view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func contentsRect(for interaction: ImageAnalysisInteraction) -> CGRect
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The associated interaction object for the contents rectangle.

## Return Value

The rectangle of the image within the view, in unit coordinates. The default return value is the unit rectangle, `[0.0, 0.0, 1.0, 1.0]`, which represents the whole view contents.

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

Implement this method when the interaction view type isn’t UIImageView.

## Default Implementations

### ImageAnalysisInteractionDelegate Implementations

func contentsRect(for: ImageAnalysisInteraction) -> CGRect

A default unit rectangle that represents the full size of the interaction view.

## See Also

### Providing interface details

func contentView(for: ImageAnalysisInteraction) -> UIView?

Provides the view that contains the image.

**Required** Default implementation provided.

func presentingViewController(for: ImageAnalysisInteraction) -> UIViewController?

Provides the view controller that presents the interface objects.

**Required** Default implementation provided.

