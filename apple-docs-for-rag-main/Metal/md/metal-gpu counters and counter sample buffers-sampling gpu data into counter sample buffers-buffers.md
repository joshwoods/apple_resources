

- Metal
- GPU Counters and Counter Sample Buffers
-  Sampling GPU Data into Counter Sample Buffers 

Article

# Sampling GPU Data into Counter Sample Buffers

Retrieve a GPU’s counter data at a time the GPU supports.

## Overview

You can sample a GPU device’s performance counter data at different times, including:

- At pipeline stage boundaries

- Between different Metal commands

Typically, a GPU supports one of these boundary types. For example, Apple silicon supports sampling at the stage boundary because it processes fragments after processing every primitive for a render pass. However, a typical immediate-mode GPU supports sampling between commands.

Before you can sample a GPU counter, implement the following prerequisite steps:

1.  Identify which counters you can sample from an MTLDevice instance (see Confirming which Counters and Counter Sets a GPU Supports).

2.  Make an MTLCounterSampleBuffer instance to store the counter’s data (see Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass).

The sections below explain how to identify when you can sample a GPU’s counters, and how to encode commands to retrieve their data.

Each GPU vendor defines its own private data format for its counter sample buffers, which means your app can’t read the contents of each buffer directly. Instead, your app can transform the data from the vendor’s internal format to Metal’s standard formats by *resolving* each sample buffer. See Converting a GPU’s Counter Data into a Readable Format for the next steps that resolve the data within a counter sample buffer.

### Check Which Boundaries a GPU Supports

You can inspect a GPU device instance to see whether it supports a specific sample boundary by calling its supportsCounterSampling(_:) method with each MTLCounterSamplingPoint case.

- Swift
- Objective-C

```
func samplingBoundariesFor(_ device: MTLDevice) -> [MTLCounterSamplingPoint] {
    let boundaryNames = ["atStageBoundary",
                         "atDrawBoundary",
                         "atBlitBoundary",
                         "atDispatchBoundary",
                         "atTileDispatchBoundary"]

    let allBoundaries: [MTLCounterSamplingPoint] = [.atStageBoundary,
                                                   .atDrawBoundary,
                                                   .atBlitBoundary,
                                                   .atDispatchBoundary,
                                                   .atTileDispatchBoundary]

    print("The GPU device supports the following sampling boundary/ies: [", terminator: "")
    var boundaries = [MTLCounterSamplingPoint]()

    for index in 0..= 1 {
                // Prefix the boundary's name with a comma and a space.
                print(", ", terminator: "")
            }

            // Print the boundary's name.
            print("\(boundaryNames[index])", terminator: "")

            // Add the boundary to the return-value array.
            boundaries.append(boundary)
        }
    }

    // Finish printing the line that lists the boundaries the GPU device supports.
    // Example: "The GPU device supports the following sampling boundaries: [atStageBoundary]"
    print("]")

    return boundaries
}
```

```
+ (NSArray*) samplingBoundariesFor:(id)device
{
    NSArray* boundaryNames = @[@"atStageBoundary",
                                          @"atDrawBoundary",
                                          @"atBlitBoundary",
                                          @"atDispatchBoundary",
                                          @"atTileDispatchBoundary"];

    NSUInteger allBoundaries[] = {
        MTLCounterSamplingPointAtStageBoundary,
        MTLCounterSamplingPointAtDrawBoundary,
        MTLCounterSamplingPointAtBlitBoundary,
        MTLCounterSamplingPointAtDispatchBoundary,
        MTLCounterSamplingPointAtTileDispatchBoundary};

    printf("The GPU device supports the following sampling boundary/ies: [");

    NSMutableArray* boundaries = [[NSMutableArray alloc] init];

    for (int index = 0; index = 1) {
                // Prefix the boundary's name with a comma and a space.
                printf(", ");
            }

            // Print the boundary's name.
            printf("%s", boundaryNames[index].UTF8String);

            // Add the boundary to the return-value array.
            NSNumber* boundaryNumber = [NSNumber numberWithUnsignedLong:allBoundaries[index]];
            [boundaries addObject: boundaryNumber];
        }
    }

    // Finish printing the line that lists the boundaries the GPU device supports.
    // Example: "The GPU device supports these sampling boundaries: [atStageBoundary]"
    printf("]\n");

    return boundaries;
}
```

This method checks for multiple sample boundaries and returns those the GPU supports in an array.

### Sample Counters at Stage Boundaries

For a GPU device that can sample counters at stage boundaries ( MTLCounterSamplingPoint.atStageBoundary), you can sample its counters between the stages of a pass. When the GPU starts or finishes a stage, it samples the counters and copies the results into a counter sample buffer.

Note

By default, a pass doesn’t sample any GPU counters.

You tell the GPU which counters to sample by configuring a pass descriptor’s sampleBufferAttachments property. For example, you can sample the timestamp counters before and after the vertex and fragment stages by configuring an MTLRenderPassDescriptor instance’s sampleBufferAttachments property.

- Swift
- Objective-C

```
func configureRenderPass(_ renderPass: MTLRenderPassDescriptor, attachmentIndex: Int = 0) {
    guard let sampleAttachment = renderPass.sampleBufferAttachments[attachmentIndex] else {
        return
    }

    sampleAttachment.sampleBuffer = self.counterSampleBuffer
    sampleAttachment.startOfVertexSampleIndex = 0
    sampleAttachment.endOfVertexSampleIndex = 1
    sampleAttachment.startOfFragmentSampleIndex = 2
    sampleAttachment.endOfFragmentSampleIndex = 3
}
```

```
- (void) configureRenderPass:(MTLRenderPassDescriptor *)renderPass
             attachmentIndex: (int)index
{
    MTLRenderPassSampleBufferAttachmentDescriptor *sampleAttachment;
    sampleAttachment = renderPass.sampleBufferAttachments[index];

    sampleAttachment.sampleBuffer = self.counterSampleBuffer;
    sampleAttachment.startOfVertexSampleIndex = 0;
    sampleAttachment.endOfVertexSampleIndex = 1;
    sampleAttachment.startOfFragmentSampleIndex = 2;
    sampleAttachment.endOfFragmentSampleIndex = 3;
}
```

Each index value tells the GPU where to put a specific counter value within a counter sample buffer. You can skip specific counters by setting an index to MTLCounterDontSample. For example, you can alter the code example above so that the GPU only samples before and after a fragment stage.

```
    ...
    sampleAttachment.sampleBuffer = self.counterSampleBuffer;
    sampleAttachment.startOfVertexSampleIndex = MTLCounterDontSample;
    sampleAttachment.endOfVertexSampleIndex = MTLCounterDontSample;
    sampleAttachment.startOfFragmentSampleIndex = 2;
    sampleAttachment.endOfFragmentSampleIndex = 3;
}
```

This example still stores the fragment counter data in the third and fourth positions within the counter sample buffer (at indexes 2 and 3, respectively). However, it doesn’t sample the vertex stage timestamps, which leaves that part of the counter sample buffer unaltered.

Each type of pass has different boundary types and corresponding properties in their descriptor types.

| Pass descriptor type | Attachment type | Attachment descriptor properties |
|----|----|----|
| MTLRenderPassDescriptor | MTLRenderPassSampleBufferAttachmentDescriptor | sampleBuffer  startOfVertexSampleIndex  endOfVertexSampleIndex  startOfFragmentSampleIndex  endOfFragmentSampleIndex |
| MTLAccelerationStructurePassDescriptor | MTLAccelerationStructurePassSampleBufferAttachmentDescriptor | sampleBuffer  startOfEncoderSampleIndex  endOfEncoderSampleIndex |
| MTLComputePassDescriptor | MTLComputePassSampleBufferAttachmentDescriptor | sampleBuffer  startOfEncoderSampleIndex  endOfEncoderSampleIndex |
| MTLBlitPassDescriptor | MTLBlitPassSampleBufferAttachmentDescriptor | sampleBuffer  startOfEncoderSampleIndex  endOfEncoderSampleIndex |
| MTLResourceStatePassDescriptor | MTLResourceStatePassSampleBufferAttachmentDescriptor | sampleBuffer  startOfEncoderSampleIndex  endOfEncoderSampleIndex |

### Sample Counters at Command Boundaries

You can encode specific commands to sample a counter’s data during a pass for a GPU that supports any of the following boundaries:

- MTLCounterSamplingPoint.atDrawBoundary

- MTLCounterSamplingPoint.atDispatchBoundary

- MTLCounterSamplingPoint.atBlitBoundary

- MTLCounterSamplingPoint.atTileDispatchBoundary

You do this by calling an encoder’s sampleCounters(sampleBuffer:sampleIndex:barrier:) method.

- Swift
- Objective-C

```
renderEncoder.drawPrimitives(type: .triangle, vertexStart: 0, vertexCount: 6)

...

// Store the GPU counter data in the sample buffer.
renderEncoder.sampleCounters(sampleBuffer: self.counterSampleBuffer,
                             sampleIndex: 0,
                             barrier: false)

...

renderEncoder.drawPrimitives(type: .triangle,
                             vertexStart: entity.offset,
                             vertexCount: entity.count)
```

```
[renderEncoder drawPrimitives:MTLPrimitiveTypeTriangle
                  vertexStart:0
                  vertexCount: 6];

...

// Store the GPU counter data in the sample buffer.
[renderEncoder sampleCountersInBuffer: self.counterSampleBuffer
                        atSampleIndex: 0
                          withBarrier: NO];

...

[renderEncoder drawPrimitives: MTLPrimitiveTypeTriangle
                  vertexStart: entity.start
                  vertexCount: entity.count];
```

The code example above encodes a sample command between two draw commands. When the GPU reaches the sample command, it samples the counters and copies the results into a counter sample buffer.

Each pass encoder type has its own version of the method.

| Pass encoder type | Sample method |
|----|----|
| MTLRenderCommandEncoder | sampleCounters(sampleBuffer:sampleIndex:barrier:) |
| MTLAccelerationStructureCommandEncoder | sampleCounters(sampleBuffer:sampleIndex:barrier:) |
| MTLComputeCommandEncoder | sampleCounters(sampleBuffer:sampleIndex:barrier:) |
| MTLBlitCommandEncoder | sampleCounters(sampleBuffer:sampleIndex:barrier:) |

The `barrier` parameter for these methods controls whether the pass waits for the GPU to complete all the previous commands in the buffer before sampling the counters (see Resource Synchronization). Each barrier typically reduces performance, but can be useful during development to get accurate and consistent data across multiple runs.

## See Also

### Counter Sample Buffers

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

Make a buffer that provides a place for a GPU to save its runtime performance metrics as it runs a pass.

class MTLCounterSampleBufferDescriptor

A group of properties that configures the counter sample buffers you create with it.

protocol MTLCounterSampleBuffer

A specialized memory buffer that stores a GPU’s counter set data.

var MTLCounterDontSample: Int

A sentinel value that instructs an encoder to skip sampling a counter as the GPU runs the encoder’s pass.

