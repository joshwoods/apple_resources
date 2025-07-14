

- HealthKit
-  HKWorkoutSession 

Class

# HKWorkoutSession

A session that tracks the user’s workout on Apple Watch.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
class HKWorkoutSession
```

## Mentioned in 

Running workout sessions

## Overview

The session fine-tunes Apple Watch’s sensors for the specified activity. All workout sessions generate high-frequency heart rate samples; however, an outdoor cycling activity generates accurate location data, while an indoor cycling activity doesn’t.

Apple Watch runs one workout session at a time. If a second workout starts while your workout is running, your HKWorkoutSessionDelegate object receives an HKError.Code.errorAnotherWorkoutSessionStarted error, and your session ends.

## Topics

### Creating workout sessions

init(healthStore: HKHealthStore, configuration: HKWorkoutConfiguration) throws

Returns a newly instantiated workout session with an associated workout builder.

### Monitoring the session

var delegate: (any HKWorkoutSessionDelegate)?

The workout session’s delegate.

protocol HKWorkoutSessionDelegate

The session delegate protocol that defines an interface for receiving notifications about errors and changes in the workout session’s state.

### Accessing the workout builder

func associatedWorkoutBuilder() -> HKLiveWorkoutBuilder

Returns the live workout builder associated with the workout session.

### Managing the workout

func prepare()

Prepares the workout session.

func startActivity(with: Date?)

Starts the workout session activity, and sets the start date.

func pause()

Pauses the workout session.

func resume()

Resumes the workout session.

func stopActivity(with: Date?)

Stops the workout session activity, and sets the end date.

func end()

Ends the workout session.

### Working with remote workout sessions

func startMirroringToCompanionDevice(completion: (Bool, (any Error)?) -> Void)

Starts mirroring the workout session to the companion iOS device.

func stopMirroringToCompanionDevice(completion: (Bool, (any Error)?) -> Void)

Stops mirroring the workout session to the companion iOS device.

func sendToRemoteWorkoutSession(data: Data, completion: (Bool, (any Error)?) -> Void)

Sends the provided data to the remote workout session.

### Accessing session data

var endDate: Date?

The ending time and date for this workout session.

var startDate: Date?

The starting time and date for this workout session.

var state: HKWorkoutSessionState

The workout session’s current state.

var type: HKWorkoutSessionType

A value that indicates whether the session is a primary session or a mirrored session.

var workoutConfiguration: HKWorkoutConfiguration

The configuration object that describes this workout.

### Managing workout activities

var currentActivity: HKWorkoutActivity

The current workout activity.

func beginNewActivity(configuration: HKWorkoutConfiguration, date: Date, metadata: [String : Any]?)

Begins a new workout activity in the workout session.

func endCurrentActivity(on: Date)

Ends the current workout activity.

### Deprecated methods

init(activityType: HKWorkoutActivityType, locationType: HKWorkoutSessionLocationType)

Returns a newly instantiated workout session.

Deprecated

init(configuration: HKWorkoutConfiguration) throws

Returns a newly instantiated workout session.

Deprecated

var activityType: HKWorkoutActivityType

The workout activity performed during this session.

Deprecated

var locationType: HKWorkoutSessionLocationType

A value that indicates whether the workout session occurred indoors or outdoors.

Deprecated

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
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Sessions

Running workout sessions

Track a workout on Apple Watch.

Build a workout app for Apple Watch

Create your own workout app, quickly and easily, with HealthKit and SwiftUI.

Building a multidevice workout app

Mirror a workout from a watchOS app to its companion iOS app, and perform bidirectional communication between them.

class HKWorkoutConfiguration

An object that contains configuration information about a workout session.

enum HKWorkoutSessionState

A workout session’s state.

class HKLiveWorkoutBuilder

A builder object that constructs a workout incrementally based on live data from an active workout session.

class HKLiveWorkoutDataSource

A data source that automatically provides live data from an active workout session.

