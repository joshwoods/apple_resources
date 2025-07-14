

- LockedCameraCapture
-  LockedCameraCaptureExtension 

Protocol

# LockedCameraCaptureExtension

A protocol that creates a locked camera capture extension.

iOS 18.0+iPadOS 18.0+

``` source
@MainActor
protocol LockedCameraCaptureExtension : AppExtension
```

## Topics

### Associated Types

associatedtype Body : LockedCameraCaptureExtensionScene

**Required**

### Instance Properties

var body: Self.Body

The content for the locked camera capture extension.

**Required**

## Relationships

### Inherits From

- AppExtension

## See Also

### Extension

protocol LockedCameraCaptureExtensionScene

A protocol that provides the UI for the locked camera capture extension.

