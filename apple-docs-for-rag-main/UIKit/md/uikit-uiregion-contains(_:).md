

- UIKit
- UIRegion
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean indicating whether the specified point is inside of the current region.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func contains(_ point: CGPoint) -> Bool
```

## Parameters 

`point`  

The point to test. The specified point must be in the region’s coordinate system.

## Return Value

true if the point is in the current region or false if it is not.

## Discussion

UIKit Dynamics normally calls this method when it needs to determine the interactions between two objects. If you call this method yourself, remember that the origin of the region object itself is at the center of the region’s shape and you might need to adjust the value of `point` accordingly.

