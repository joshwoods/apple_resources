

- BrowserEngineKit
- BEScrollViewScrollUpdate
-  translation(in:) 

Instance Method

# translation(in:)

Returns the amount of scrolling in the scroll update in the given view’s coordinates.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func translation(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view in which to find the scroll amount. Pass `nil` to get the amount in the window’s coordinate system.

## Return Value

The amount of scrolling in the scroll update in the specified view.

## Overview

If either the `x` or `y` value of the returned point is non-zero, then the scroll update represents a change large enough to be visible along that axis.

## See Also

### Transforming coordinates

func location(in: UIView?) -> CGPoint

Returns the coordinates of the scroll update in the given view’s bounds.

