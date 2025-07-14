

- LockedCameraCapture
-  LockedCameraCaptureManager 

Class

# LockedCameraCaptureManager

An object that provides handling of captured content and transitioning to the extension’s containing app.

iOS 18.0+iPadOS 18.0+

``` source
final class LockedCameraCaptureManager
```

## Topics

### Instance Properties

var sessionContentURLs: [URL]

An array of URLs that each point to a directory containing captured content.

var sessionContentUpdates: some AsyncSequence&lt;LockedCameraCaptureManager.SessionContentUpdate, Never>

An `AsyncSequence` to process captured content from your capture extension.

### Instance Methods

func beginDelayingAppearance()

Tells the system that the application wants to delay the application launch during a transition between the extension and the application

func endDelayingAppearance()

Tells the system that the application is ready to appear after delaying the appearance during a transition between the extension and the application

func invalidateSessionContent(at: URL) async throws

Tells the system that the app no longer needs the directory at the URL and it can be deleted.

### Type Properties

static let shared: LockedCameraCaptureManager

The shared instance of the manager.

### Enumerations

enum SessionContentUpdate

URLs provided by the sessionContentUpdates `AsyncSequence`.

## Relationships

### Conforms To

- Sendable

## See Also

### App integration

let NSUserActivityTypeLockedCameraCapture: String

A type to use when opening your app from the capture extension.

