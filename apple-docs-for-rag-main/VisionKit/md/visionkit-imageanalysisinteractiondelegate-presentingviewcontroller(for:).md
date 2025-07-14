

- VisionKit
- ImageAnalysisInteractionDelegate
-  presentingViewController(for:) 

Instance Method

# presentingViewController(for:)

Provides the view controller that presents the interface objects.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func presentingViewController(for interaction: ImageAnalysisInteraction) -> UIViewController?
```

**Required** Default implementation provided.

## Parameters 

`interaction`  

The associated interaction object for the presented view.

## Return Value

The view controller that presents the interaction object’s highlights, menus, and other elements.

## Discussion

The default return value is the window’s root view controller.

## Default Implementations

### ImageAnalysisInteractionDelegate Implementations

func presentingViewController(for: ImageAnalysisInteraction) -> UIViewController?

A default implementation that provides the interaction view’s root view controller.

## See Also

### Providing interface details

func contentView(for: ImageAnalysisInteraction) -> UIView?

Provides the view that contains the image.

**Required** Default implementation provided.

func contentsRect(for: ImageAnalysisInteraction) -> CGRect

Returns the rectangle, in unit coordinates, that contains the image within the view.

**Required** Default implementation provided.

