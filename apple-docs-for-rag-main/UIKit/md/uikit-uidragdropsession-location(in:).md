

- UIKit
- UIDragDropSession
-  location(in:) 

Instance Method

# location(in:)

Returns the geometrical location of the user’s drag activity within the specified view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func location(in view: UIView) -> CGPoint
```

**Required**

## Parameters 

`view`  

The view whose coordinate system is used to get the location.

## Return Value

The location point of the drag activity, in the coordinate system of the specified view.

