

- UIKit
- UISpringLoadedInteractionContext
-  location(in:) 

Instance Method

# location(in:)

Returns the location of the drag activity within the specified view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func location(in view: UIView?) -> CGPoint
```

**Required**

## Parameters 

`view`  

The view that is used to determine the location of the drag activity.

## Return Value

A point in the local coordinate system of `view`.

## Discussion

To get the location of the drag activity within the window, use `nil` for the view.

