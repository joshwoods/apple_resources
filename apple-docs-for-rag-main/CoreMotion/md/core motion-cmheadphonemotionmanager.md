

- Core Motion
-  CMHeadphoneMotionManager 

Class

# CMHeadphoneMotionManager

An object that starts and manages headphone motion services.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
class CMHeadphoneMotionManager
```

## Mentioned in 

Getting processed device-motion data

## Overview

This class delivers headphone motion updates to your app. Use an instance of the manager to determine if the device supports motion, and to start and stop updates. Adopt the CMHeadphoneMotionManagerDelegate protocol to receive and respond to motion updates. Before using this class, check isDeviceMotionAvailable to make sure the feature is available.

Important

In iOS and macOS, include the NSMotionUsageDescription key in your app’s `Info.plist` file. If this key is absent, the system crashes your app when you start device-motion updates.

### Identify the coordinate axes

To interpret attitude data, you need to know the orientation of the device’s coordinate axes. The following illustration shows the positive x-axis, positive y-axis, and positive z-axis for motion-capable Apple headphones.

## Topics

### Checking Availability

var isDeviceMotionAvailable: Bool

A Boolean value that indicates whether the current device supports the headphone motion manager.

var isDeviceMotionActive: Bool

A Boolean value that indicates whether the headphone motion manager is active.

var isConnectionStatusActive: Bool

class func authorizationStatus() -> CMAuthorizationStatus

Returns the authorization status for monitoring headphone motion.

### Starting and Stopping Updates

func startDeviceMotionUpdates()

Starts device-motion updates.

func startDeviceMotionUpdates(to: OperationQueue, withHandler: CMHeadphoneMotionManager.DeviceMotionHandler)

Starts device-motion updates with a handler.

func startConnectionStatusUpdates()

func stopDeviceMotionUpdates()

Stops device-motion updates.

func stopConnectionStatusUpdates()

### Getting the Delegate

var delegate: (any CMHeadphoneMotionManagerDelegate)?

The object that receives headphone motion manager events.

protocol CMHeadphoneMotionManagerDelegate

A set of methods that defines an interface for connecting and disconnecting headphones.

### Getting Device-Motion Information

var deviceMotion: CMDeviceMotion?

The latest device-motion data.

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

### Device motion

Getting processed device-motion data

Retrieve motion data that the system processed to remove environmental bias, such as the effects of gravity.

class CMDeviceMotion

Encapsulated measurements of the attitude, rotation rate, and acceleration of a device.

class CMAttitude

The device’s orientation relative to a known frame of reference at a point in time.

struct CMAttitudeReferenceFrame

Constants that indicate the frame of reference for attitude-related motion data.

