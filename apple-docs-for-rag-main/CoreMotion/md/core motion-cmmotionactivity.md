

- Core Motion
-  CMMotionActivity 

Class

# CMMotionActivity

The data for a single motion update event.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 15.0+watchOS 2.0+

``` source
class CMMotionActivity
```

## Overview

On devices that support motion, you can use a CMMotionActivityManager or CMHeadphoneActivityManager object to request updates when the current type of motion changes. When a change occurs, the update information is packaged into a CMMotionActivity object and sent to your app.

The motion-related properties of this class aren’t mutually exclusive. In other words, it’s possible for more than one of the motion-related properties to contain the value true. For example, if the user was driving in a car and the car stopped at a red light, the update event associated with that change in motion would have both the automotive and stationary properties set to true. It’s also possible for all of the properties to be set to false when the device is in motion but the movement doesn’t correlate to walking, running, cycling, or automotive travel.

You don’t create instances of this class yourself. The CMMotionActivityManager object creates them and sends them to the handler block you registered. For more information about how to initiate the delivery of motion activity updates to your app, see CMMotionActivityManager.

## Topics

### Getting the Type of Motion

var stationary: Bool

A Boolean indicating whether the device is stationary.

var walking: Bool

A Boolean indicating whether the device is on a walking person.

var running: Bool

A Boolean indicating whether the device is on a running person.

var automotive: Bool

A Boolean indicating whether the device is in an automobile.

var cycling: Bool

A Boolean indicating whether the device is in a bicycle.

var unknown: Bool

A Boolean indicating whether the type of motion is unknown.

### Getting Metadata for the Motion

var startDate: Date

The time at which the change in motion occurred.

var confidence: CMMotionActivityConfidence

The confidence in the assessment of the motion type.

enum CMMotionActivityConfidence

The confidence that the motion data is accurate.

## Relationships

### Inherits From

- CMLogItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Activity

class CMMotionActivityManager

An object that manages access to the motion data stored by the device.

class CMHeadphoneActivityManager

An object that starts and manages headphone activity services.

Getting motion-activity data from headphones

Configure your app to listen for motion-activity changes from headphones.

