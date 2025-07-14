

- SensorKit
-  SRDeviceUsageReport 

Class

# SRDeviceUsageReport

The frequency and relative duration that the user uses their device, particular Apple apps, or websites.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRDeviceUsageReport
```

## Overview

The deviceUsageReport sensor provides this class as its sample type.

## Topics

### Summarizing Device Use

var duration: TimeInterval

The duration that the report spans.

var totalScreenWakes: Int

The total number of screen wakes for the device.

var totalUnlocks: Int

The total number of unlocks for the device.

var totalUnlockDuration: TimeInterval

The duration of time the device is in an unlocked state.

### Analyzing App Use

var applicationUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.ApplicationUsage]]

The usage time of apps per category.

class ApplicationUsage

An object that describes the user’s app activity over a period of time.

struct CategoryKey

Categories of apps or websites that the user uses.

### Analyzing Notification Use

var notificationUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.NotificationUsage]]

The frequency of notifications per category.

class NotificationUsage

An object that describes notification frequency and the manner in which the user interacts with notifications.

### Analyzing Web Use

var webUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.WebUsage]]

The amount of time the user accesses domains per category.

class WebUsage

An object that describes a user’s website usage.

### Getting algorithm information

var version: String

The version of the algorithm that the system uses to generate the report.

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

### Interpreting data

class SRAmbientLightSample

The amount of ambient light in the user’s environment.

class SRKeyboardMetrics

The configuration of a device’s keyboard and its usage patterns.

class SRMediaEvent

A user interaction with a media object, such as an image or a video.

class SRMessagesUsageReport

An object that describes the user’s Messages app activity over a period of time.

class SRPhoneUsageReport

An object that describes the user’s phone activity over a period of time.

class SRVisit

The user’s progress in their daily travel routine.

class SRWristDetection

The configuration of a watch on the wearer’s wrist.

