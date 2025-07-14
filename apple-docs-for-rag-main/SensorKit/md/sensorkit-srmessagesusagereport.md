

- SensorKit
-  SRMessagesUsageReport 

Class

# SRMessagesUsageReport

An object that describes the user’s Messages app activity over a period of time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRMessagesUsageReport
```

## Overview

This object describes the frequency that the user sends or receives messages, and the relative amount of time the user uses the Messages app.

The messagesUsageReport sensor provides this class as its sample type.

## Topics

### Analyzing Message Use

var duration: TimeInterval

The duration that the report spans.

var totalIncomingMessages: Int

The number of messages the user receives.

var totalOutgoingMessages: Int

The number of messages the user sends.

var totalUniqueContacts: Int

The user’s number of contacts.

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

class SRDeviceUsageReport

The frequency and relative duration that the user uses their device, particular Apple apps, or websites.

class SRKeyboardMetrics

The configuration of a device’s keyboard and its usage patterns.

class SRMediaEvent

A user interaction with a media object, such as an image or a video.

class SRPhoneUsageReport

An object that describes the user’s phone activity over a period of time.

class SRVisit

The user’s progress in their daily travel routine.

class SRWristDetection

The configuration of a watch on the wearer’s wrist.

