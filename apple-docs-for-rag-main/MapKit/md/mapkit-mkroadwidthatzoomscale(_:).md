

- MapKit
-  MKRoadWidthAtZoomScale(\_:) 

Function

# MKRoadWidthAtZoomScale(\_:)

Returns the width (in screen points) of roads on a map at the specified zoom level.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func MKRoadWidthAtZoomScale(_ zoomScale: MKZoomScale) -> CGFloat
```

## Parameters 

`zoomScale`  

The scale factor currently applied to the map view.

## Return Value

The width of roads, measured in screen points. You can use the returned value to set the width of lines in drawing code that traces the path of a road.

## See Also

### Types

typealias MKZoomScale

A scale factor to use in conjunction with a map.

