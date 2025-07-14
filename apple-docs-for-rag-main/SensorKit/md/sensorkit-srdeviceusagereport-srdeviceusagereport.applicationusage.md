

- SensorKit
- SRDeviceUsageReport
-  SRDeviceUsageReport.ApplicationUsage 

Class

# SRDeviceUsageReport.ApplicationUsage

An object that describes the user’s app activity over a period of time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class ApplicationUsage
```

## Overview

Each instance of this class represents an app in a particular app category. For more information, see applicationUsageByCategory.

## Topics

### Identifying the App

var bundleIdentifier: String?

The bundle identifier of the app in use.

var reportApplicationIdentifier: String

A pseudonymn for a real application identifier.

var supplementalCategories: [SRSupplementalCategory]

Categories that provide more information about an app.

class SRSupplementalCategory

A more detailed category that provides additional context to the app category.

### Timing App Use

var usageTime: TimeInterval

The amount of time the user uses the app.

var relativeStartTime: TimeInterval

The time the user starts the app relative to the start time of the first app in a report interval.

### Inspecting Text Input

var textInputSessions: [SRTextInputSession]

The text input session types that occur during application usage.

class SRTextInputSession

The characters a user types for a particular keyboard.

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

### Analyzing App Use

var applicationUsageByCategory: [SRDeviceUsageReport.CategoryKey : [SRDeviceUsageReport.ApplicationUsage]]

The usage time of apps per category.

struct CategoryKey

Categories of apps or websites that the user uses.

