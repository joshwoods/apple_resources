

- SwiftUI
- MeshGradient
-  init(width:height:points:colors:background:smoothsColors:colorSpace:) 

Initializer

# init(width:height:points:colors:background:smoothsColors:colorSpace:)

Creates a new gradient mesh specified as a 2D grid of colored points.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    width: Int,
    height: Int,
    points: [SIMD2],
    colors: [Color],
    background: Color = .clear,
    smoothsColors: Bool = true,
    colorSpace: Gradient.ColorSpace = .device
)
```

## Parameters 

`width`  

The width of the mesh, i.e. the number of vertices per row.

`height`  

The height of the mesh, i.e. the number of vertices per column.

`points`  

The array of points, containing `width x height` elements.

`colors`  

The array of colors, containing `width x height` elements.

`background`  

The background color, this fills any points outside the defined vertex mesh.

`smoothsColors`  

Whether cubic (smooth) interpolation should be used for the colors in the mesh (rather than only for the shape of the mesh).

`colorSpace`  

The color space in which to interpolate vertex colors.

