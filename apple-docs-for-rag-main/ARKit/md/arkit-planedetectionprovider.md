

- ARKit
-  PlaneDetectionProvider 

Class

# PlaneDetectionProvider

A source of live data about planes in a person’s surroundings.

visionOS 1.0+

``` source
final class PlaneDetectionProvider
```

## Overview

Use this provider to indicate to ARKit the types of plane anchors for your app to detect.

## Topics

### Detecting planes

init(alignments: [PlaneAnchor.Alignment])

Creates a plane detection provider for the types of planes you want to detect.

var allAnchors: [PlaneAnchor]

An array that contains all the plane provider’s anchors.

var anchorUpdates: AnchorUpdateSequence&lt;PlaneAnchor>

A sequence of updates to planes a provider detects.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for detecting planes.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports plane detection providers.

### Inspecting a plane detection provider

var alignments: [PlaneAnchor.Alignment]

The plane alignments that you configure a provider to detect.

var state: DataProviderState

The current status of data coming from a provider.

var description: String

A textual representation of this plane detection provider.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Plane detection

Placing content on detected planes

Detect horizontal surfaces like tables and floors, as well as vertical planes like walls and doors.

struct PlaneAnchor

An anchor that represents horizontal and vertical planes.

