

- HealthKit
-  HKWorkoutConfiguration 

Class

# HKWorkoutConfiguration

An object that contains configuration information about a workout session.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
class HKWorkoutConfiguration
```

## Overview

Like many HealthKit classes, the HKWorkoutConfiguration class is not extendable and should not be subclassed.

## Topics

### Session settings

var activityType: HKWorkoutActivityType

The workout session’s activity type.

var locationType: HKWorkoutSessionLocationType

The workout session’s location.

enum HKWorkoutSessionLocationType

A constant indicating whether the workout session takes place indoors or outdoors.

var swimmingLocationType: HKWorkoutSwimmingLocationType

The workout session’s swimming location.

enum HKWorkoutSwimmingLocationType

The possible locations for swimming.

var lapLength: HKQuantity?

The length of the lap for a workout session.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

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

enum HKWorkoutSessionState

A workout session’s state.

class HKLiveWorkoutBuilder

A builder object that constructs a workout incrementally based on live data from an active workout session.

class HKLiveWorkoutDataSource

A data source that automatically provides live data from an active workout session.

