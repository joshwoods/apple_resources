

- Video Toolbox
-  VTRAWProcessingSession 

Class

# VTRAWProcessingSession

An object that processes frames in camera native formats such as RAW or Bayer.

macOS 15.0+

``` source
class VTRAWProcessingSession
```

## Overview

A RAW processing session supports processing of frames that have been output from decoders in camera native formats, such as RAW or Bayer formats.

The session reference is a reference-counted CF object.

## Topics

### Configuring parameters

func parameters() -> any AsyncSequence&lt;[VTRAWProcessingSession.Parameter], Never>

Returns an asynchronous sequence that provides updates to the processing Parameter array if the processing extension makes changes to the set of Parameters.

func updateParameter(values: [String : Any]) throws

Sets the value for one or more of the processing parameters.

var processingParameters: [VTRAWProcessingSession.Parameter]

An array of processing parameters available for this RAW processing session.

enum Parameter

A parameter expresses a control or a set of controls that influence frame processing.

### Processing frames

func process(frame: CVPixelBuffer) async throws -> CVPixelBuffer

Processes an input pixel buffer.

### Configuring the Metal device

var metalDevice: (any MTLDevice)?

The preferred device to use for any Metal-based processing performed by the RAW Processing Extension.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

