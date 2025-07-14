

- BrowserEngineKit
- BEScrollViewScrollUpdate
-  location(in:) 

Instance Method

# location(in:)

Returns the coordinates of the scroll update in the given view’s bounds.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func location(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view in which to find the scroll update location. Pass `nil` to get the location in the window’s coordinate system.

## Return Value

The location of the scroll update in the specified view.

## See Also

### Transforming coordinates

func translation(in: UIView?) -> CGPoint

Returns the amount of scrolling in the scroll update in the given view’s coordinates.

