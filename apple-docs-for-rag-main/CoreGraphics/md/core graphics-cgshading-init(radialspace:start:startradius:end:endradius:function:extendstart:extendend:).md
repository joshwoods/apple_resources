

- Core Graphics
- CGShading
-  init(radialSpace:start:startRadius:end:endRadius:function:extendStart:extendEnd:) 

Initializer

# init(radialSpace:start:startRadius:end:endRadius:function:extendStart:extendEnd:)

Creates a shading object to use for radial shading.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    radialSpace space: CGColorSpace,
    start: CGPoint,
    startRadius: CGFloat,
    end: CGPoint,
    endRadius: CGFloat,
    function: CGFunction,
    extendStart: Bool,
    extendEnd: Bool
)
```

## Parameters 

`space`  

The color space in which color values are expressed. Core Graphics retains this object; upon return, you may safely release it.

`start`  

The center of the starting circle, in the shading’s target coordinate space.

`startRadius`  

The radius of the starting circle, in the shading’s target coordinate space.

`end`  

The center of the ending circle, in the shading’s target coordinate space.

`endRadius`  

The radius of the ending circle, in the shading’s target coordinate space.

`function`  

A CGFunction object created by the function init(info:domainDimension:domain:rangeDimension:range:callbacks:). This object refers to your function for creating a radial shading. Core Graphics retains this object; upon return, you may safely release it.

`extendStart`  

A Boolean value that specifies whether to extend the shading beyond the starting circle.

`extendEnd`  

A Boolean value that specifies whether to extend the shading beyond the ending circle.

## Return Value

A new Core Graphics radial shading. In Objective-C, you’re responsible for releasing this object using CGShadingRelease.

## Discussion

A radial shading is a color blend that varies between two circles. To draw the shading, call the function drawShading(_:).

## See Also

### Creating Shading Objects

init?(axialSpace: CGColorSpace, start: CGPoint, end: CGPoint, function: CGFunction, extendStart: Bool, extendEnd: Bool)

Creates a shading object to use for axial shading.

