

- HealthKit
-  HKUpdateFrequency 

Enumeration

# HKUpdateFrequency

Constants that determine how often the system launches your app in response to changes to HealthKit data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKUpdateFrequency
```

## Overview

For more information, see HKObserverQuery.

## Topics

### Constants

case immediate

The system launches your app every time it detects a change.

case hourly

The system launches your app at most once an hour in response to changes.

case daily

The system launches your app at most once a day in response to changes.

case weekly

The system launches your app at most once per week in response to changes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing background delivery

func enableBackgroundDelivery(for: HKObjectType, frequency: HKUpdateFrequency, withCompletion: (Bool, (any Error)?) -> Void)

Enables the delivery of updates to an app running in the background.

com.apple.developer.healthkit.background-delivery

A Boolean value that indicates whether observer queries receive updates while running in the background.

func disableBackgroundDelivery(for: HKObjectType, withCompletion: (Bool, (any Error)?) -> Void)

Disables background deliveries of update notifications for the specified data type.

func disableAllBackgroundDelivery(completion: (Bool, (any Error)?) -> Void)

Disables all background deliveries of update notifications.

