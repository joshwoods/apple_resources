

- LockedCameraCapture
-  LockedCameraCaptureSession 

Class

# LockedCameraCaptureSession

An object that can request to open the extension’s containing app and receives session configuration updates.

iOS 18.0+iPadOS 18.0+

``` source
final class LockedCameraCaptureSession
```

## Overview

Provided during the initialization of the LockedCameraCaptureExtensionScene. Only the system can initialize this object.

## Topics

### Instance Properties

var sessionContentURL: URL

A temporary directory URL inside the extension’s data container.

### Instance Methods

func invalidateSessionContent() async throws

Invalidates the contents of the session contents URL, deleting them. Note this does not remove the contents directory itself. This is useful in case the extension has already ingested its contents via PhotoKit and wishes to not persist any data (but can still use this directory as a working directory to recover from an unexpected termination).

func openApplication(for: NSUserActivity) async throws

Initiates a request to open the extension’s containing app.

### Enumerations

enum ApplicationLaunchError

Indicates why launching the extension’s containing app failed.

## Relationships

### Conforms To

- Sendable

## See Also

### Capture and launch

struct LockedCameraCaptureUIScene

A structure that contains the session object and UI to display for the locked camera capture extension.

