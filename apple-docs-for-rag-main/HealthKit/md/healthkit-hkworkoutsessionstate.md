

- HealthKit
-  HKWorkoutSessionState 

Enumeration

# HKWorkoutSessionState

A workout session’s state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
enum HKWorkoutSessionState
```

## Topics

### Session states

case notStarted

The workout session has not started.

case prepared

The session is ready but not yet running.

case running

The workout session is running.

case paused

The workout session has paused.

case stopped

The session has stopped.

case ended

The workout session has ended.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Sessions

Running workout sessions

Track a workout on Apple Watch.

Build a workout app for Apple Watch

Create your own workout app, quickly and easily, with HealthKit and SwiftUI.

Building a multidevice workout app

Mirror a workout from a watchOS app to its companion iOS app, and perform bidirectional communication between them.

class HKWorkoutSession

A session that tracks the user’s workout on Apple Watch.

class HKWorkoutConfiguration

An object that contains configuration information about a workout session.

class HKLiveWorkoutBuilder

A builder object that constructs a workout incrementally based on live data from an active workout session.

class HKLiveWorkoutDataSource

A data source that automatically provides live data from an active workout session.

