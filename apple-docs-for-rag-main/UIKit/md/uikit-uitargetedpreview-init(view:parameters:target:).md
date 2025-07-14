

- UIKit
- UITargetedPreview
-  init(view:parameters:target:) 

Initializer

# init(view:parameters:target:)

Creates a targeted preview with the specified view, parameters, and target container.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
init(
    view: UIView,
    parameters: UIPreviewParameters,
    target: UIPreviewTarget
)
```

## Parameters 

`view`  

The view to animate.

`parameters`  

The animation parameters.

`target`  

The container for the view.

## Return Value

A new targeted preview object.

## See Also

### Creating a targeted preview object

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

convenience init(view: UIView, parameters: UIPreviewParameters)

Creates a targeted preview for a view in the current window and including the specified parameters.

convenience init(view: UIView)

Creates a targeted preview for a view in the current window.

