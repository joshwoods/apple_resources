

- Metal
- MTLCounterSamplingPoint
-  MTLCounterSamplingPoint.atStageBoundary 

Case

# MTLCounterSamplingPoint.atStageBoundary

Counter sampling is allowed at the start and end of a render pass’s vertex and fragment stages, and at the start and end of compute and blit passes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
case atStageBoundary
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## See Also

### Reading Sampling Boundary Types

case atBlitBoundary

Counter sampling is allowed between blit commands in a blit pass.

case atDispatchBoundary

Counter sampling is allowed between kernel dispatches in a compute pass.

case atDrawBoundary

Counter sampling is allowed between draw commands in a render pass.

case atTileDispatchBoundary

Counter sampling is allowed between tile dispatches in a render pass.

