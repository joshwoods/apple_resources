

- Core Motion
-  CMStepCounter Deprecated

Class

# CMStepCounter

The number of steps the user has taken with the device.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class CMStepCounter
```

Deprecated

Use the CMPedometer class instead.

## Overview

Step information is gathered on devices with the appropriate built-in hardware and stored so that you can run queries to determine the user’s recent physical activity. You use this class to gather both current step data and any historical data.

## Topics

### Determining Step Counting Availability

class func isStepCountingAvailable() -> Bool

Returns a Boolean indicating whether step-counting support is available on the current device.

### Starting and Stopping Step Counting Updates

func startStepCountingUpdates(to: OperationQueue, updateOn: Int, withHandler: CMStepUpdateHandler)

Starts the delivery of current step-counting data to your app.

func stopStepCountingUpdates()

Stops the delivery of step-counting updates to your app.

typealias CMStepUpdateHandler

A block that reports the number of steps recorded since updates began.

### Getting Historical Step Counting Data

func queryStepCountStarting(from: Date, to: Date, to: OperationQueue, withHandler: CMStepQueryHandler)

Gathers and returns historical step count data for the specified time period.

typealias CMStepQueryHandler

A block that reports the number of steps for a query operation.

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

### Pedometer and fitness

class CMPedometer

An object for fetching the system-generated live walking data.

class CMPedometerData

Information about the distance traveled by a user on foot.

class CMPedometerEvent

A change in the user’s pedestrian activity.

class CMOdometerData

A class that represents odometer data for workouts.

class CMHighFrequencyHeartRateData

A class that represents heart rate data collected at 1 Hz.

