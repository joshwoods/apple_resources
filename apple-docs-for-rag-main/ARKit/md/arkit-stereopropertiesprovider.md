

- ARKit
-  StereoPropertiesProvider 

Class

# StereoPropertiesProvider

The StereoPropertiesProvider serves the latest viewpoint properties on the device.

visionOS 2.4+

``` source
final class StereoPropertiesProvider
```

## Topics

### Initializers

init()

Initialize the StereoPropertiesProvider.

### Instance Properties

var description: String

A textual representation of this stereo properties provider.

var latestViewpointProperties: ViewpointProperties?

Returns the latest viewpoint properties, if available.

var state: DataProviderState

The state of this stereo properties provider.

### Type Properties

static var isSupported: Bool

Determines whether this device supports the stereo properties provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The authorization type(s) required by the stereo properties provider.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

