

- ScreenCaptureKit
-  SCStreamConfiguration 

Class

# SCStreamConfiguration

An instance that provides the output configuration for a stream.

Mac Catalyst 18.2+macOS 12.3+

``` source
class SCStreamConfiguration
```

## Overview

Creating an instance of this class provides a default configuration for a stream. Only configure its properties if you need to customize the output.

## Topics

### Specifying dimensions

var width: Int

The width of the output.

var height: Int

The height of the output.

var scalesToFit: Bool

A Boolean value that indicates whether to scale the output to fit the configured width and height.

var sourceRect: CGRect

A rectangle that specifies the source area to capture.

var destinationRect: CGRect

A rectangle that specifies a destination into which to write the output.

var preservesAspectRatio: Bool

A Boolean value that determines if the stream preserves aspect ratio.

### Configuring colors

var pixelFormat: OSType

A pixel format for sample buffers that a stream outputs.

var colorMatrix: CFString

A color matrix to apply to the output surface.

var colorSpaceName: CFString

A color space to use for the output buffer.

var backgroundColor: CGColor

A background color for the output.

### Configuring captured elements

var showsCursor: Bool

A Boolean value that determines whether the cursor is visible in the stream.

var shouldBeOpaque: Bool

A Boolean value that indicates if semitransparent content presents as opaque.

var capturesShadowsOnly: Bool

A Boolean value that indicates if the stream only captures shadows.

var ignoreShadowsDisplay: Bool

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in display style.

var ignoreShadowsSingleWindow: Bool

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in window style.

var ignoreGlobalClipDisplay: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in display style.

var ignoreGlobalClipSingleWindow: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in window style.

### Configuring captured frames

var queueDepth: Int

The maximum number of frames for the queue to store.

var minimumFrameInterval: CMTime

The desired minimum time between frame updates, in seconds.

var captureResolution: SCCaptureResolutionType

The resolution at which to capture source content.

enum SCCaptureResolutionType

Available resolutions for content capture.

### Configuring audio

var capturesAudio: Bool

A Boolean value that indicates whether to capture audio.

var sampleRate: Int

The sample rate for audio capture.

var channelCount: Int

The number of audio channels to capture.

var excludesCurrentProcessAudio: Bool

A Boolean value that indicates whether to exclude audio from your app during capture.

### Identifying a stream

var streamName: String?

A name that you provide for identifying the stream.

### Notifying presenters

var presenterOverlayPrivacyAlertSetting: SCPresenterOverlayAlertSetting

A value indicating if alerts appear to presenters while using Presenter Overlay.

enum SCPresenterOverlayAlertSetting

Configures how to present streaming notifications to a streamer of Presenter Overlay.

### Enumerations

enum SCCaptureDynamicRange

enum Preset

### Initializers

convenience init(preset: SCStreamConfiguration.Preset)

### Instance Properties

var captureDynamicRange: SCCaptureDynamicRange

var captureMicrophone: Bool

var includeChildWindows: Bool

var microphoneCaptureDeviceID: String?

var showMouseClicks: Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Content capture

class SCStream

An instance that represents a stream of shareable content.

class SCContentFilter

An instance that filters the content a stream captures.

protocol SCStreamDelegate

A delegate protocol your app implements to respond to stream events.

class SCScreenshotManager

An instance for the capture of single frames from a stream.

