

- Video Toolbox
-  VTFrameSilo 

API Collection

# VTFrameSilo

An object that stores sample buffers from a multipass encoding session.

## Overview

A frame silo object starts out empty and is populated by calls to VTFrameSiloAddSampleBuffer(_:sampleBuffer:) to add sample buffers in ascending decode order. After the first full pass, additional passes may be performed to replace sample buffers. Each such pass must begin with a call to VTFrameSiloSetTimeRangesForNextPass(_:timeRangeCount:timeRangeArray:), which takes a list of time ranges. Samples in these time ranges are deleted, and calls to VTFrameSiloAddSampleBuffer(_:sampleBuffer:) can then be made to provide replacements.

Call VTFrameSiloCallFunctionForEachSampleBuffer(_:in:refcon:callback:) or VTFrameSiloCallBlockForEachSampleBuffer(_:in:handler:) to retrieve sample buffers. The frame silo object may write sample buffers and data to the backing file between addition and retrieval; don’t expect to get identical object pointers back.

The sample buffers are ordered by decode timestamp.

## Topics

### Creating Frame Silos

func VTFrameSiloCreate(allocator: CFAllocator?, fileURL: CFURL?, timeRange: CMTimeRange, options: CFDictionary?, frameSiloOut: UnsafeMutablePointer&lt;VTFrameSilo?>) -> OSStatus

Creates a frame silo object using a temporary file.

### Configuring Frame Silos

func VTFrameSiloAddSampleBuffer(VTFrameSilo, sampleBuffer: CMSampleBuffer) -> OSStatus

Adds a sample buffer to a frame silo object.

func VTFrameSiloSetTimeRangesForNextPass(VTFrameSilo, timeRangeCount: CMItemCount, timeRangeArray: UnsafePointer&lt;CMTimeRange>) -> OSStatus

Begins a new pass of samples to be added to a frame silo object.

func VTFrameSiloCallBlockForEachSampleBuffer(VTFrameSilo, in: CMTimeRange, handler: (CMSampleBuffer) -> OSStatus) -> OSStatus

Retrieves sample buffers from a frame silo object.

func VTFrameSiloCallFunctionForEachSampleBuffer(VTFrameSilo, in: CMTimeRange, refcon: UnsafeMutableRawPointer?, callback: (UnsafeMutableRawPointer?, CMSampleBuffer) -> OSStatus) -> OSStatus

Retrieves sample buffers from a frame silo object.

### Inspecting Frame Silos

func VTFrameSiloGetProgressOfCurrentPass(VTFrameSilo, progressOut: UnsafeMutablePointer&lt;Float32>) -> OSStatus

Gets the progress of the current pass.

func VTFrameSiloGetTypeID() -> CFTypeID

Retrieves the Core Foundation type identifier for the frame silo object.

### Data Types

class VTFrameSilo

An object that stores a large number of sample buffers, as produced by a multipass compression session.

## See Also

### Compression

Encoding video for low-latency conferencing

Configure a compression session to optimize encoding for video-conferencing apps.

Encoding video for live streaming

Configure a compression session to encode video for live streaming.

Encoding video for offline transcoding

Configure a compression session to transcode video in offline workflows.

VTCompressionSession

An object that compresses video data.

VTDecompressionSession

An object that decompresses video data.

VTMultiPassStorage

An object that stores video encoding metadata from a multipass encoding session.

