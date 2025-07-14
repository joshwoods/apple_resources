

- ScreenCaptureKit
-  SCStreamDelegate 

Protocol

# SCStreamDelegate

A delegate protocol your app implements to respond to stream events.

Mac Catalyst 18.2+macOS 12.3+

``` source
protocol SCStreamDelegate : NSObjectProtocol
```

## Topics

### Responding to Presenter Overlay

func outputVideoEffectDidStart(for: SCStream)

Tells the delegate that Presenter Overlay started.

func outputVideoEffectDidStop(for: SCStream)

Tells the delegate that Presenter Overlay stopped.

### Responding to stream stoppage

func stream(SCStream, didStopWithError: any Error)

Tells the delegate that the stream stopped with an error.

### Instance Methods

func streamDidBecomeActive(SCStream)

func streamDidBecomeInactive(SCStream)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Content capture

class SCStream

An instance that represents a stream of shareable content.

class SCStreamConfiguration

An instance that provides the output configuration for a stream.

class SCContentFilter

An instance that filters the content a stream captures.

class SCScreenshotManager

An instance for the capture of single frames from a stream.

