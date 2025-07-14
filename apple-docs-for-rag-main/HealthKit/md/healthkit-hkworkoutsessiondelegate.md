

- HealthKit
-  HKWorkoutSessionDelegate 

Protocol

# HKWorkoutSessionDelegate

The session delegate protocol that defines an interface for receiving notifications about errors and changes in the workout session’s state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
protocol HKWorkoutSessionDelegate : NSObjectProtocol
```

## Mentioned in 

Running workout sessions

## Overview

All the methods are required. HealthKit calls these methods on an anonymous serial background queue.

## Topics

### Tracking workout sessions

func workoutSession(HKWorkoutSession, didChangeTo: HKWorkoutSessionState, from: HKWorkoutSessionState, date: Date)

Tells the delegate that the session’s state changed.

**Required**

func workoutSession(HKWorkoutSession, didFailWithError: any Error)

Tells the delegate that the session failed with an error.

**Required**

func workoutSession(HKWorkoutSession, didGenerate: HKWorkoutEvent)

Tells the delegate that the system generated a workout event.

func workoutSession(HKWorkoutSession, didBeginActivityWith: HKWorkoutConfiguration, date: Date)

Tells the delegate that a new workout session began.

func workoutSession(HKWorkoutSession, didEndActivityWith: HKWorkoutConfiguration, date: Date)

Tells the session that the current workout activity ended.

### Working with mirrored sessions

func workoutSession(HKWorkoutSession, didDisconnectFromRemoteDeviceWithError: (any Error)?)

Tells the delegate that the mirrored workout session disconnected from the primary session.

func workoutSession(HKWorkoutSession, didReceiveDataFromRemoteWorkoutSession: [Data])

Passes data from the remote workout session to the session delegate.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Monitoring the session

var delegate: (any HKWorkoutSessionDelegate)?

The workout session’s delegate.

