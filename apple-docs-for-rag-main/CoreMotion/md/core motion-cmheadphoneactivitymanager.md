

- Core Motion
-  CMHeadphoneActivityManager 

Class

# CMHeadphoneActivityManager

An object that starts and manages headphone activity services.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
class CMHeadphoneActivityManager
```

## Overview

This class delivers headphone activity updates to your app. Use an instance of the manager to determine if the device supports headphone activity updates, and to start and stop updates. Before using this class, check isActivityAvailable and isStatusAvailable to make sure the features are available.

This class provides similar information to CMMotionActivityManager, except the activity information comes from headphone motion, rather than from device motion.

Important

In iOS and macOS, include the NSMotionUsageDescription key in your app’s `Info.plist` file. If this key is absent, trying to start headphone activity updates terminates your app.

## Topics

### Checking Availability

var isActivityAvailable: Bool

A Boolean value that indicates whether the current device supports headphone activity.

var isActivityActive: Bool

A Boolean value that indicates whether headphone motion activity is active.

var isStatusAvailable: Bool

A Boolean value that indicates whether the current device supports headphone status.

var isStatusActive: Bool

A Boolean value that indicates whether headphone status is active.

class func authorizationStatus() -> CMAuthorizationStatus

Returns the authorization status for monitoring headphone activity.

### Starting and Stopping Updates

func startActivityUpdates(to: OperationQueue, withHandler: CMHeadphoneActivityManager.ActivityHandler)

Starts headphone activity updates, providing data to the given handler through the given queue.

func stopActivityUpdates()

Stops headphone activity updates.

func startStatusUpdates(to: OperationQueue, withHandler: CMHeadphoneActivityManager.StatusHandler)

Starts headphone status updates, providing data to the given handler through the given queue.

func stopStatusUpdates()

Stops headphone status updates.

### Supporting Types

enum Status

Headphone connection status updates.

typealias ActivityHandler

The type for a handler to be invoked when headphone motion activity data is available.

typealias StatusHandler

The type for a handler to be invoked with status updates.

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

class CMMotionActivityManager

An object that manages access to the motion data stored by the device.

class CMMotionActivity

The data for a single motion update event.

Getting motion-activity data from headphones

Configure your app to listen for motion-activity changes from headphones.

