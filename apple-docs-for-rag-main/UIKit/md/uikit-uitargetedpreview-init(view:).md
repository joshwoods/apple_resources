

- UIKit
- UITargetedPreview
-  init(view:) 

Initializer

# init(view:)

Creates a targeted preview for a view in the current window.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
convenience init(view: UIView)
```

## Parameters 

`view`  

The view to animate. This view must be in a window.

## Return Value

A new targeted preview object.

## See Also

### Creating a targeted preview object

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

init(view: UIView, parameters: UIPreviewParameters, target: UIPreviewTarget)

Creates a targeted preview with the specified view, parameters, and target container.

convenience init(view: UIView, parameters: UIPreviewParameters)

Creates a targeted preview for a view in the current window and including the specified parameters.

