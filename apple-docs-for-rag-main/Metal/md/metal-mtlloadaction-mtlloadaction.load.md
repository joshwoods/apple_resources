

- Metal
- MTLLoadAction
-  MTLLoadAction.load 

Case

# MTLLoadAction.load

The GPU preserves the existing contents of the attachment at the start of the render pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case load
```

## Mentioned in 

Setting Load and Store Actions

## See Also

### Constants

case dontCare

The GPU has permission to discard the existing contents of the attachment at the start of the render pass, replacing them with arbitrary data.

case clear

The GPU writes a value to every pixel in the attachment at the start of the render pass.

