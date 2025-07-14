

- Metal
- MTLStencilOperation
-  MTLStencilOperation.incrementWrap 

Case

# MTLStencilOperation.incrementWrap

If the current stencil value is not the maximum representable value, increase the stencil value by one. Otherwise, if the current stencil value is the maximum representable value, set the stencil value to zero.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case incrementWrap
```

## See Also

### Constants

case keep

Keep the current stencil value.

case zero

Set the stencil value to zero.

case replace

Replace the stencil value with the stencil reference value, which is set by the setStencilReferenceValue(_:) method of MTLRenderCommandEncoder.

case incrementClamp

If the current stencil value is not the maximum representable value, increase the stencil value by one. Otherwise, if the current stencil value is the maximum representable value, do not change the stencil value.

case decrementClamp

If the current stencil value is not zero, decrease the stencil value by one. Otherwise, if the current stencil value is zero, do not change the stencil value.

case invert

Perform a logical bitwise invert operation on the current stencil value.

case decrementWrap

If the current stencil value is not zero, decrease the stencil value by one. Otherwise, if the current stencil value is zero, set the stencil value to the maximum representable value.

