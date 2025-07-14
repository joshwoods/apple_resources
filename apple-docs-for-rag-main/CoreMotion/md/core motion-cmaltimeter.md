

- Core Motion
-  CMAltimeter 

Class

# CMAltimeter

An object that initiates the delivery of altitude-related changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class CMAltimeter
```

## Overview

Altitude events report changes in both the relative and absolute altitude. For example, a hiking app could use this object to track the user’s elevation change over the course of a hike, or to report their current absolute altitude during the hike.

Because altitude events may not be available on all devices, always call the isRelativeAltitudeAvailable() method before starting relative altitude updates, and call isAbsoluteAltitudeAvailable() before starting absolute altitude updates.

After checking the availability of altitude data, call the startRelativeAltitudeUpdates(to:withHandler:) method to start receiving relative altitude data, or call the startAbsoluteAltitudeUpdates(to:withHandler:) method for absolute altitude data.

Core Motion generates events at regular intervals (regardless of whether the data has changed) and delivers them to the block you specified. When you no longer need the event data, call the stopRelativeAltitudeUpdates() or stopAbsoluteAltitudeUpdates() methods respectively.

Important

To use this API, you must include the NSMotionUsageDescription key in your app’s `Info.plist` file and provide a usage description string for this key. The usage description appears in the prompt that the user must accept the first time the system asks the user to access motion data for your app. If you don’t include a usage description string, your app crashes when you call this API.

## Topics

### Determining Altitude Availability

class func isAbsoluteAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device reports changes in the absolute altitude.

class func isRelativeAltitudeAvailable() -> Bool

Returns a Boolean value indicating whether the current device supports generating data for relative altitude changes.

class func authorizationStatus() -> CMAuthorizationStatus

Returns a value indicating whether the app is authorized to retrieve altimeter data.

enum CMAuthorizationStatus

The authorization status for motion-related features.

### Starting and Stopping Altitude Updates

func startAbsoluteAltitudeUpdates(to: OperationQueue, withHandler: CMAbsoluteAltitudeHandler)

Starts the delivery of absolute altitude data to the specified handler.

func stopAbsoluteAltitudeUpdates()

Stops the delivery of absolute altitude data for this altimeter object.

typealias CMAbsoluteAltitudeHandler

A block for receiving absolute altitude data.

func startRelativeAltitudeUpdates(to: OperationQueue, withHandler: CMAltitudeHandler)

Starts the delivery of relative altitude data to the specified handler.

func stopRelativeAltitudeUpdates()

Stops the delivery of relative altitude data for the altimeter object.

typealias CMAltitudeHandler

A block for receiving relative altitude data.

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

### Altitude data

class CMAbsoluteAltitudeData

Data that records a change in absolute altitude.

class CMAltitudeData

Data for a recorded change in altitude.

