

- HealthKit
- Workouts and activity rings
-  Building a multidevice workout app 

Sample Code

# Building a multidevice workout app

Mirror a workout from a watchOS app to its companion iOS app, and perform bidirectional communication between them.

Download

iOS 17.0+iPadOS 17.0+watchOS 10.0+Xcode 15.0+

## Overview

Note

This sample code project is associated with WWDC23 session 10023: Build a multidevice workout app.

### Configure the sample code project

This sample code project needs to run on physical devices. Before you run it with Xcode:

- Set the developer team for all targets to let Xcode automatically manage the provisioning profile. For more information, see Assign a project to a team.

- In the Info pane of the `MirroringWorkoutsSample Watch App` target, change the value of the `WKCompanionAppBundleIdentifier` key to the bundle ID of the iOS app.

## See Also

### Sessions

Running workout sessions

Track a workout on Apple Watch.

Build a workout app for Apple Watch

Create your own workout app, quickly and easily, with HealthKit and SwiftUI.

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

