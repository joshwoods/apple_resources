

- MapKit
- MKPolygonRenderer
-  init(polygon:) 

Initializer

# init(polygon:)

Creates a new renderer that handles drawing for the specified polygon overlay object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
init(polygon: MKPolygon)
```

## Parameters 

`polygon`  

The polygon overlay containing information about the area the polygon renderer draws. This object requires at least three points defining the polygon to draw. This parameter can’t be `nil`.

## Return Value

An initialized polygon renderer object.

