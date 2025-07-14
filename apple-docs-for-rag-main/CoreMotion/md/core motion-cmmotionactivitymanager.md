

- Core Motion
-  CMMotionActivityManager 

Class

# CMMotionActivityManager

An object that manages access to the motion data stored by the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class CMMotionActivityManager
```

## Overview

Motion data reflects whether the user is walking, running, in a vehicle, or stationary for periods of time. Using this class, you can ask for notifications when the current type of motion changes or you can gather past motion change data. For example, a navigation app might look for changes in the current type of motion and offer different directions for each.

Important

To use this API, you must include the NSMotionUsageDescription key in your app’s `Info.plist` file and provide a usage description string for this key. The usage description appears in the prompt that the user must accept the first time the system asks the user to access motion data for your app. If you don’t include a usage description string, your app crashes when you call this API.

## Topics

### Determining Activity Availability

class func isActivityAvailable() -> Bool

Returns a Boolean indicating whether motion data is available on the current device.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to retrieve stored motion data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

### Starting and Stopping Activity Updates

func startActivityUpdates(to: OperationQueue, withHandler: CMMotionActivityHandler)

Starts the delivery of current motion data updates to your app.

func stopActivityUpdates()

Stops the delivery of motion updates to your app

typealias CMMotionActivityHandler

A block that reports the current motion associated with the device.

### Getting Historical Activity Data

func queryActivityStarting(from: Date, to: Date, to: OperationQueue, withHandler: CMMotionActivityQueryHandler)

Gathers and returns historical motion data for the specified time period

typealias CMMotionActivityQueryHandler

A block that reports the motion updates that occurred between the specified query interval.

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

## See Also

### Activity

class CMHeadphoneActivityManager

An object that starts and manages headphone activity services.

class CMMotionActivity

The data for a single motion update event.

Getting motion-activity data from headphones

Configure your app to listen for motion-activity changes from headphones.

