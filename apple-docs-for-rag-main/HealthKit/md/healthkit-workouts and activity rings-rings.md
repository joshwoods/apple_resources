

- HealthKit
-  Workouts and activity rings 

API Collection

# Workouts and activity rings

Manage workouts, workout sessions, and activity summaries.

## Overview

A workout is a sample that contains data about an exercise or fitness activity. You save workout data using the HKWorkout class. In many ways, workouts are identical to any other HealthKit sample—the same advice and APIs apply to both workouts and samples. However, workouts do have a number of unique features, described in HKWorkout.

Workout sessions let you track the user’s activity on Apple Watch. While a workout session is active, your app can continue to run in the background. This lets your app monitor the user and gather data throughout the activity. Additionally, it ensures that your app appears whenever the user checks their watch. After the session ends, your app saves the activity’s data as a workout sample. For more information on setting up and running workout sessions, see HKWorkoutSession.

The Activity Rings display a summary of the user’s daily activity on Apple Watch and in the Activity app. Activity summaries provide access to the data displayed in the user’s Move, Exercise, and Stand rings. To see how your workout samples contribute to these rings, see Fill the Activity rings. To learn more about accessing and displaying activity data in your app, see Activity rings.

Finally, workout routes record the user’s path during an outdoor activity (for example, while walking, running, or cycling). Routes can be associated with a workout sample. For more information, see Creating a workout route and Reading route data.

## Topics

### Samples

Adding samples to a workout

Create associated samples that add details to a workout.

Accessing condensed workout samples

Read series data from condensed workouts.

Dividing a HealthKit workout into activities

Partition multisport and interval workouts into activities that represent the different parts of the workout.

class HKWorkout

A workout sample that stores information about a single physical activity.

class HKWorkoutActivity

An object that describes an activity within a longer workout.

class HKWorkoutBuilder

A builder object that incrementally constructs a workout.

class HKWorkoutType

A type that identifies samples that store information about a workout.

let HKWorkoutTypeIdentifier: String

The workout type identifier.

enum HKWorkoutActivityType

The type of activity performed during a workout.

enum HKWorkoutSessionType

The type of session.

class HKWorkoutEvent

An object representing an important event during a workout.

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

enum HKWorkoutSessionState

A workout session’s state.

class HKLiveWorkoutBuilder

A builder object that constructs a workout incrementally based on live data from an active workout session.

class HKLiveWorkoutDataSource

A data source that automatically provides live data from an active workout session.

### Activity rings

class HKActivitySummary

An object that contains the move, exercise, and stand data for a given day.

struct HKActivitySummaryQueryDescriptor

A query interface that reads activity summaries using Swift concurrency.

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

class HKActivityRingView

A view that uses the Move, Exercise, and Stand activity rings to display data from a HealthKit activity summary object.

class HKActivityMoveModeObject

An object that contains a movement mode value.

### Route data

Creating a workout route

Record the user’s route during a workout.

Reading route data

Access the user’s route for a workout.

class HKWorkoutRouteBuilder

A builder object that incrementally constructs a workout route.

class HKWorkoutRoute

A sample that contains a workout’s route data.

struct HKWorkoutRouteQueryDescriptor

A query interface that reads the location data stored in a workout route using Swift concurrency.

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

let HKWorkoutRouteTypeIdentifier: String

A series sample containing location data that defines the route the user took during a workout.

class HKSeriesBuilder

An abstract base class for building series samples.

class HKSeriesSample

An abstract base class that defines samples that contain a series of items.

