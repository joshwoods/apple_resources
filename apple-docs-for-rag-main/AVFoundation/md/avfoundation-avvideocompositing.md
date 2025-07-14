

- AVFoundation
-  AVVideoCompositing 

Protocol

# AVVideoCompositing

A protocol that defines the methods custom video compositors must implement.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
protocol AVVideoCompositing : NSObjectProtocol, Sendable
```

## Overview

For each AVFoundation object of class AVPlayerItem, AVAssetExportSession, AVAssetImageGenerator, or AVAssetReaderVideoCompositionOutput that has a non-`nil` value for its `videoComposition` property, and the value of the customVideoCompositorClass property of the `AVVideoComposition` isn’t `nil`, AVFoundation creates and uses an instance of that custom video compositor class to process the instructions contained in the AVVideoComposition.

The system creates a custom video compositor instance when you assign `videoComposition` an instance of AVVideoComposition that’s associated with a different custom video compositor class than the object was previously using.

When creating instances of custom video compositors, AVFoundation initializes them by calling `init` and then makes them available as the value of the `customVideoCompositor` property of the object. You then can do any additional setup or configuration to the custom compositor.

The AVFoundation object retains the custom video compositor instances for as long as the value of the `videoComposition` property indicates that there’s an instance of the same custom video compositor class. This is true even when the value changes from one instance of AVVideoComposition to another associated instance with the same custom video compositor class.

## Topics

### Inspecting Processing Requirements

var sourcePixelBufferAttributes: [String : any Sendable]?

The pixel buffer attributes that the compositor accepts for source frames.

**Required**

var requiredPixelBufferAttributesForRenderContext: [String : any Sendable]

The pixel buffer attributes that the compositor requires for pixel buffers that it creates.

**Required**

var supportsHDRSourceFrames: Bool

A Boolean value that indicates whether the compositor handles source frames that contain high dynamic range (HDR) properties.

var supportsWideColorSourceFrames: Bool

A Boolean value that indicates whether the compositor handles source frames that contains wide color properties.

var canConformColorOfSourceFrames: Bool

A Boolean value that indicates whether the compositor conforms the color space of source frames to the composition color space.

### Observing Render Context Changes

func renderContextChanged(AVVideoCompositionRenderContext)

Tells the compositor that the composition changed render contexts.

**Required**

class AVVideoCompositionRenderContext

An object that defines the context in which custom compositors render pixel buffers.

### Preparing to Render Frames

func anticipateRendering(using: AVVideoCompositionRenderHint)

Informs a custom video compositor about upcoming rendering requests.

func prerollForRendering(using: AVVideoCompositionRenderHint)

Tells a custom video compositor to perform any work in the prerolling phase.

class AVVideoCompositionRenderHint

Information about upcoming composition requests, such as composition start time and end time.

### Rendering the Composition

func startRequest(AVAsynchronousVideoCompositionRequest)

Directs a custom video compositor object to create a new pixel buffer composed asynchronously from a collection of sources.

**Required**

class AVAsynchronousVideoCompositionRequest

An object that contains information a video compositor needs to render an output pixel buffer.

func cancelAllPendingVideoCompositionRequests()

Directs a custom video compositor object to cancel or finish all pending video composition requests.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

