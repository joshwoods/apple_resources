

- UIKit
- UIContextMenuInteraction
-  location(in:) 

Instance Method

# location(in:)

Returns the location of the user interaction in the specified view’s coordinate system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func location(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view containing the target coordinate system. To return a point in the window’s coordinate system, specify `nil`.

## Return Value

The location of the interaction specified in the coordinate system of `view`.

