

- UIKit
-  UIUpdateInfo 

Class

# UIUpdateInfo

An object that contains detailed information about the current UI update state.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class UIUpdateInfo
```

## Overview

During a UI update, this object provides details about the state of the update. When using a UIUpdateLink, you can query this UI update information object to learn about the current UI update.

A UI update can service views on different displays simultaneously, which means these views can have a different UIUpdateInfo. Get the UI update information for a specific view using current(for:) or a specific window using current(for:). The UI update information can also change as the current UI update progresses through its phases.

## Topics

### Getting the current UI update information

class func current(for: UIView) -> Self?

Returns an object that describes the current UI update state for the specified view.

class func current(for: UIWindowScene) -> Self?

Returns an object that describes the current UI update state for the specified window.

### Getting information about timing

var modelTime: TimeInterval

The time interval that represents a reference point for the current time of the UI update.

var completionDeadlineTime: TimeInterval

The time interval that represents the time by which an app needs to finish submitting changes to the render server.

var estimatedPresentationTime: TimeInterval

The time interval that represents an estimate for when current UI update changes become visible onscreen.

### Working with low-latency updates

var isImmediatePresentationExpected: Bool

A Boolean value that indicates whether the system presents UI updates immediately upon completion.

var isLowLatencyEventDispatchConfirmed: Bool

A Boolean value that indicates whether the system runs low-latency phases for the UI update.

var isPerformingLowLatencyPhases: Bool

A Boolean value that indicates whether the UI update is in the low-latency phases.

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

## See Also

### UI updates

class UIUpdateLink

An object you use to observe, participate in, and affect the UI update process.

class UIUpdateActionPhase

An object that defines specific phases of the UI update process.

