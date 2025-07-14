

- VisionKit
- ImageAnalysisInteractionDelegate
-  contentView(for:) 

Instance Method

# contentView(for:)

Provides the view that contains the image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func contentView(for interaction: ImageAnalysisInteraction) -> UIView?
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The associated interaction object for the content view.

## Return Value

The view that contains the image for this interaction.

## Discussion

Implement this delegate method only when the view that contains the image isn’t the same as the interaction’s view.

## Default Implementations

### ImageAnalysisInteractionDelegate Implementations

func contentView(for: ImageAnalysisInteraction) -> UIView?

A default implementation that provides the interaction’s view.

## See Also

### Providing interface details

func contentsRect(for: ImageAnalysisInteraction) -> CGRect

Returns the rectangle, in unit coordinates, that contains the image within the view.

**Required** Default implementation provided.

func presentingViewController(for: ImageAnalysisInteraction) -> UIViewController?

Provides the view controller that presents the interface objects.

**Required** Default implementation provided.

