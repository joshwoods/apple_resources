

- AVFoundation
-  AVRouteDetector 

Class

# AVRouteDetector

An object that detects available media playback routes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class AVRouteDetector
```

## Mentioned in 

Supporting AirPlay in your app

## Overview

If you enable route detection, the object reports whether it detects multiple playback routes. If it does, use AVRoutePickerView to present the UI for the user to select an appropriate route.

## Topics

### Detecting Routes

var detectsCustomRoutes: Bool

A Boolean value that indicates whether route detection includes custom routes.

var isRouteDetectionEnabled: Bool

A Boolean value that indicates whether route detection is in an enabled state.

var multipleRoutesDetected: Bool

A Boolean value that indicates whether the object detects more than one playback route.

static let AVRouteDetectorMultipleRoutesDetectedDidChange: NSNotification.Name

A notification the system posts when changes occur to its detected routes.

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
- Sendable

