

- UIKit
- UIPreviewTarget
-  init(container:center:) 

Initializer

# init(container:center:)

Creates a preview target object using the specified container view and center point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    container: UIView,
    center: CGPoint
)
```

## Parameters 

`container`  

The container for the view being animated. This view must be in a window.

`center`  

The point in `container` at which to place the center of the view being animated. Specify this point in the coordinate system of `container`.

## Return Value

A new preview target object with the specified container and configuration data.

## See Also

### Creating a preview target object

init(container: UIView, center: CGPoint, transform: CGAffineTransform)

Creates a preview target object using the specified container view and configuration details.

