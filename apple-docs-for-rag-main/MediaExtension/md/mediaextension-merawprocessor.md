

- MediaExtension
-  MERAWProcessor 

Protocol

# MERAWProcessor

A protocol that defines the requirements for a RAW processor.

macOS 15.0+

``` source
protocol MERAWProcessor : NSObjectProtocol
```

## Overview

This protocol provides an interface for Video Toolbox to create and interact with MediaExtension RAW processors. MERAWProcessor objects are instantiated by Video Toolbox and are closely linked to a corresponding MEVideoDecoder object that produces RAW video output.

Note

Developers who wish to build MediaExtension RAW processors using this API need to include a RAW processor entitlement, provisioning profile, and specialized dictionary in their Info.plist file when building their extensions.

For more information, see Entitlements, Create a development provisioning profile, and RAW processor property list dictionary.

Once a user installs and runs the host app, embedded RAW processor extensions become available to any app on the user’s system that opts in to using them by calling VTRegisterProfessionalVideoWorkflowVideoDecoders().

Important

`MERAWProcessor` objects run in a sandboxed process without access to the filesystem, network, and other kernel resources.

MediaExtension RAW processor’s operation and life cycle closely tie to VTRAWProcessingSession.

### Creating a raw processor

An instance of the MERAWProcessorExtension factory object is created the first time the given processor is opened by Video Toolbox in a process. The makeProcessor(formatDescription:pixelBufferManager:) method on the MERAWProcessorExtension object will be called once for each processor instance needed. The processor can evaluate the provided CMVideoFormatDescription at this point and confirm whether it is able to process the specified format. If the processor cannot process the format, the factory routine should return MEError.Code.unsupportedFeature. This sequence of calls will happen inside of VTRAWProcessingSession.

### Configuring pixel buffer requirements

At any point after instantiation, the processor can call back into the provided MERAWProcessorPixelBufferManager object to notify Video Toolbox of its output pixel buffer requirements. The processor extension may make multiple calls if output requirements change in response to properties being set or due to observed bitstream characteristics.

### Processing frames

Calls to processFrame(fromImageBuffer:completionHandler:) are serialized. A new frame is not sent to the processor until the last processFrame(fromImageBuffer:completionHandler:) has returned, but may be submitted before the processFrame(fromImageBuffer:completionHandler:) completion handler is called if the processing is happening asynchronously. These calls correspond to VTRAWProcessingSessionProcessFrame calls on the parent `VTRAWProcessingSession`.

RAW processors must write their output frames into `CVPixelBuffers` allocated through the makePixelBuffer() interface. Returning CVPixelBuffer from any other source may result in degraded performance or other issues.

If the processor’s internal processing queue is full, and it cannot process more frames, it should return NO when the isReadyForMoreMediaData property is queried. This property should return YES again when the processor is able to accept new frames – generally after an earlier asynchronous frame processing operation is completed.

## Topics

### Inspecting a RAW processor

var metalDeviceRegistryID: UInt64

Requests the processor use the provided Metal device for processing.

var outputColorAttachments: [String : Any]

Returns the color-related Core Video image buffer keys and values that become attachments to the output pixel buffers.

var processingParameters: [MERAWProcessingParameter]

Provides a list of processing parameters that can be changed by the client of Video Toolbox session to influence processing behavior.

**Required**

var isReadyForMoreMediaData: Bool

Indicates the readiness of the processor to accept more sample buffers.

**Required**

### Processing RAW frame

func processFrame(fromImageBuffer: CVPixelBuffer, completionHandler: (CVPixelBuffer?, (any Error)?) -> Void)

Requests the processor to process a video frame.

**Required**

### Extension requirements

RAW processor property list dictionary

Include a property list dictionary to describe a RAW processor.

RAW processor entitlement

Include an entitlement to indicate your extension is a MediaExtension RAW processor.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### RAW processors

protocol MERAWProcessorExtension

A protocol that defines a factory to create RAW processors for a codec type that the extension implements.

class MERAWProcessorPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

class MERAWProcessingParameter

An object for the RAW processor to describe each processing parameter the processor exposes.

enum MERAWProcessorNotification

Notifications that indicate a RAW processor state change.

RAW processor property list dictionary

Include a property list dictionary to describe a RAW processor.

RAW processor entitlement

Include an entitlement to indicate your extension is a MediaExtension RAW processor.

