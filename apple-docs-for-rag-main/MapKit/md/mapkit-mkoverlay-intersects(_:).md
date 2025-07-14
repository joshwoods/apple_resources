

- MapKit
- MKOverlay
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Returns a Boolean value that indicates whether the specified rectangle intersects the overlay’s shape.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
optional func intersects(_ mapRect: MKMapRect) -> Bool
```

## Parameters 

`mapRect`  

The rectangle to intersect with the overlay’s area.

## Return Value

true if any part of the map rectangle intersects the receiver’s shape, or false if it doesn’t.

## Discussion

You can implement this method to provide more specific bounds-checking for an overlay. If you don’t implement it, the method uses the bounding rectangle to detect intersections.

