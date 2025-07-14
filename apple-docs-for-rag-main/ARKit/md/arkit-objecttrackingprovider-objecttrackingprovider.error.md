

- ARKit
- ObjectTrackingProvider
-  ObjectTrackingProvider.Error 

Structure

# ObjectTrackingProvider.Error

Values that represent an object-tracking error.

visionOS 2.0+

``` source
struct Error
```

## Topics

### Describing an error

var code: ObjectTrackingProvider.Error.Code

The error code.

enum Code

The enumeration of object-tracking provider error codes.

var errorDescription: String?

A localized message that describes an error.

var failureReason: String?

A localized message that describes the reason for the failure.

### Inspecting an error

let bundle: Bundle?

The bundle for the model that failed to load, if the source was a bundle.

let name: String?

The name of the model that failed to load, if the source was a bundle.

var recoverySuggestion: String?

A localized message that describes how to recover from the failure.

let url: URL?

The URL for the model that failed to load, if the source was a URL.

### Instance Properties

var description: String

A textual representation of an error.

## Relationships

### Conforms To

- CustomStringConvertible
- Error
- LocalizedError
- Sendable

## See Also

### Inspecting an object-tracking provider

var state: DataProviderState

The state of an object-tracking provider.

var allAnchors: [ObjectAnchor]

An array of all the object anchors the object-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;ObjectAnchor>

An asynchronous sequence of anchors the framework updates.

var description: String

A textual representation of this object tracking provider.

