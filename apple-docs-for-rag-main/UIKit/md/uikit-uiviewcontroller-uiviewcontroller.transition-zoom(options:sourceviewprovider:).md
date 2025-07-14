

- UIKit
- UIViewController
- UIViewController.Transition
-  zoom(options:sourceViewProvider:) 

Type Method

# zoom(options:sourceViewProvider:)

Creates a zoom transition from the view that the source provider specifies.

iOS 18.0+iPadOS 18.0+Mac CatalysttvOSvisionOS

``` source
static func zoom(
    options: UIViewController.Transition.ZoomOptions? = nil,
    sourceViewProvider: @escaping (UIViewController.Transition.ZoomSourceViewProviderContext) -> UIView?
) -> Self
```

## Parameters 

`options`  

Additional options for the zoom transition.

`sourceViewProvider`  

A closure that returns the view, for example a thumbnail image, that the animation zooms out from and zooms back in to.

## Mentioned in 

Enhancing your app with fluid transitions

## Discussion

The system calls the source view provider when it presents and when it dismisses the view controller. In the closure, return the UIView that the animation should zoom in from or zoom back out to, respectively. For more information, see Enhancing your app with fluid transitions.

## See Also

### Creating zoom transitions

class ZoomOptions

Options for a zoom transition.

class ZoomSourceViewProviderContext

A context object that contains references to the view controllers from a zoom transition.

