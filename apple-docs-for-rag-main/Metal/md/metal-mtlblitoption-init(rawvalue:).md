

- Metal
- MTLBlitOption
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a blit option from a raw value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(rawValue: UInt)
```

## Parameters 

`rawValue`  

The bitwise value of a blit option as an integer.

## Discussion

Use one of the MTLBlitOption type’s static properties, such as depthFromDepthStencil, stencilFromDepthStencil, and rowLinearPVRTC instead of creating a blit option yourself with this initializer.

