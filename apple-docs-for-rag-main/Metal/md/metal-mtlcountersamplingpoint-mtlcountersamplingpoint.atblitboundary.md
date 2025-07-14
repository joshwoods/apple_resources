

- Metal
- MTLCounterSamplingPoint
-  MTLCounterSamplingPoint.atBlitBoundary 

Case

# MTLCounterSamplingPoint.atBlitBoundary

Counter sampling is allowed between blit commands in a blit pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
case atBlitBoundary
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Discussion

When a Metal device object supports this sampling boundary, you can call the sampleCounters(sampleBuffer:sampleIndex:barrier:) method on a MTLBlitCommandEncoder to sample the counters between individual blit commands.

## See Also

### Reading Sampling Boundary Types

case atDispatchBoundary

Counter sampling is allowed between kernel dispatches in a compute pass.

case atDrawBoundary

Counter sampling is allowed between draw commands in a render pass.

case atStageBoundary

Counter sampling is allowed at the start and end of a render pass’s vertex and fragment stages, and at the start and end of compute and blit passes.

case atTileDispatchBoundary

Counter sampling is allowed between tile dispatches in a render pass.

