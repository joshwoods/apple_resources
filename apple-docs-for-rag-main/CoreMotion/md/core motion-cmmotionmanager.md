

- Core Motion
-  CMMotionManager 

Class

# CMMotionManager

The object for starting and managing motion services.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
class CMMotionManager
```

## Mentioned in 

Getting raw accelerometer events

Getting raw gyroscope events

Getting processed device-motion data

## Overview

Use a CMMotionManager object to start the services that report movement detected by the device’s onboard sensors. Use this object to receive four types of motion data:

- **Accelerometer data**, indicating the instantaneous acceleration of the device in three dimensional space.

- **Gyroscope data**, indicating the instantaneous rotation around the device’s three primary axes.

- **Magnetometer data**, indicating the device’s orientation relative to Earth’s magnetic field.

- **Device-motion data**, indicating key motion-related attributes such as the device’s user-initiated acceleration, its attitude, rotation rates, orientation relative to calibrated magnetic fields, and orientation relative to gravity. Core Motion’s sensor fusion algorithms provide this data.

The processed device-motion data gives the device’s attitude, rotation rate, calibrated magnetic fields, the direction of gravity, and the amount of acceleration the user contributes to the device.

Important

Create only one CMMotionManager object for your app. Multiple instances of this class can affect the rate at which the system receives data from the accelerometer and gyroscope.

You can receive live sensor data at a specified update interval, or you can let the sensors collect data and store it for retrieval later. With both of these approaches, call the appropriate stop method (stopAccelerometerUpdates(), stopGyroUpdates(), stopMagnetometerUpdates(), and stopDeviceMotionUpdates()) when you no longer need the data.

### Receive regular motion updates

To receive motion data at specific intervals, the app calls a start method that takes an operation queue (instance of OperationQueue) and a block handler of a specific type for processing those updates. The motion data is passed into the block handler. The frequency of updates is determined by the value of an interval property.

- **Accelerometer.** Set the accelerometerUpdateInterval property to specify an update interval. Call the startAccelerometerUpdates(to:withHandler:) method, passing in a block of type CMAccelerometerHandler. Accelerometer data is passed into the block as CMAccelerometerData objects.

- **Gyroscope.** Set the gyroUpdateInterval property to specify an update interval. Call the startGyroUpdates(to:withHandler:) method, passing in a block of type CMGyroHandler. Rotation-rate data is passed into the block as CMGyroData objects.

- **Magnetometer.** Set the magnetometerUpdateInterval property to specify an update interval. Call the startMagnetometerUpdates(to:withHandler:) method, passing a block of type CMMagnetometerHandler. Magnetic-field data is passed into the block as CMMagnetometerData objects.

- **Device motion.** Set the deviceMotionUpdateInterval property to specify an update interval. Call the startDeviceMotionUpdates(using:)or startDeviceMotionUpdates(using:to:withHandler:) or startDeviceMotionUpdates(to:withHandler:) method, passing in a block of type CMDeviceMotionHandler. With the former method, you can specify a reference frame to be used for the attitude estimates. Rotation-rate data is passed into the block as CMDeviceMotion objects.

### Sample motion data periodically

To sample motion data periodically, start a motion service using a method that takes no parameters and periodically access the properties of the CMMotionManager. This approach is the recommended approach for apps such as games. Handling accelerometer data in a block introduces additional overhead, and most game apps are only interested in the latest sample of motion data when they render a frame.

- **Accelerometer.** Call startAccelerometerUpdates() to begin updates and periodically access CMAccelerometerData objects by reading the accelerometerData property.

- **Gyroscope.** Call startGyroUpdates() to begin updates and periodically access CMGyroData objects by reading the gyroData property.

- **Magnetometer.** Call startMagnetometerUpdates() to begin updates and periodically access CMMagnetometerData objects by reading the magnetometerData property.

- **Device motion.** Call the startDeviceMotionUpdates(using:) or startDeviceMotionUpdates() method to begin updates and periodically access CMDeviceMotion objects by reading the deviceMotion property. The startDeviceMotionUpdates(using:) method lets you specify a reference frame for the attitude estimates.

### Determine hardware availability and state

If a hardware feature (for example, a gyroscope) is not available on a device, calling a start method related to that feature has no effect. You can find out whether a hardware feature is available or active by checking the appropriate property; for example, for gyroscope data, you can check the value of the isGyroAvailable or isGyroActive properties.

### Identify the coordinate axes of the device

To interpret accelerometer, gyroscope, or attitude information, you need to know the orientation of the device’s coordinate axes. The following illustration shows the positive x-axis, positive y-axis, and positive z-axis for motion-capable Apple devices.

## Topics

### Determining the Availability of Services

var isDeviceMotionAvailable: Bool

A Boolean value that indicates whether the device-motion service is available on the device.

var isAccelerometerAvailable: Bool

A Boolean value that indicates whether an accelerometer is available on the device.

var isGyroAvailable: Bool

A Boolean value that indicates whether a gyroscope is available on the device.

var isMagnetometerAvailable: Bool

A Boolean value that indicates whether a magnetometer is available on the device.

### Determining Which Services Are Active

var isDeviceMotionActive: Bool

A Boolean value that determines whether the app is receiving updates from the device-motion service.

var isAccelerometerActive: Bool

A Boolean value that indicates whether accelerometer updates are currently happening.

var isGyroActive: Bool

A Boolean value that determines whether gyroscope updates are currently happening.

var isMagnetometerActive: Bool

A Boolean value that determines whether magnetometer updates are currently happening.

### Managing Device Motion Updates

var showsDeviceMovementDisplay: Bool

Controls whether the device-movement display is shown.

var deviceMotionUpdateInterval: TimeInterval

The interval, in seconds, for providing device-motion updates to the block handler.

func startDeviceMotionUpdates(using: CMAttitudeReferenceFrame, to: OperationQueue, withHandler: CMDeviceMotionHandler)

Starts device-motion updates on an operation queue and using a specified reference frame and block handler.

func startDeviceMotionUpdates(to: OperationQueue, withHandler: CMDeviceMotionHandler)

Starts device-motion updates on an operation queue and using a specified block handler.

func startDeviceMotionUpdates(using: CMAttitudeReferenceFrame)

Starts device-motion updates using a reference frame but without a block handler.

func startDeviceMotionUpdates()

Starts device-motion updates without a block handler.

func stopDeviceMotionUpdates()

Stops device-motion updates.

var deviceMotion: CMDeviceMotion?

The latest sample of device-motion data.

typealias CMDeviceMotionHandler

The type of block callback for handling device-motion data.

### Managing Accelerometer Updates

var accelerometerUpdateInterval: TimeInterval

The interval, in seconds, for providing accelerometer updates to the block handler.

func startAccelerometerUpdates(to: OperationQueue, withHandler: CMAccelerometerHandler)

Starts accelerometer updates on an operation queue and with a specified handler.

func startAccelerometerUpdates()

Starts accelerometer updates without a handler.

func stopAccelerometerUpdates()

Stops accelerometer updates.

var accelerometerData: CMAccelerometerData?

The latest sample of accelerometer data.

typealias CMAccelerometerHandler

The type of block callback for handling accelerometer data.

### Managing Gyroscope Updates

var gyroUpdateInterval: TimeInterval

The interval, in seconds, for providing gyroscope updates to the block handler.

func startGyroUpdates(to: OperationQueue, withHandler: CMGyroHandler)

Starts gyroscope updates on an operation queue and with a specified handler.

func startGyroUpdates()

Starts gyroscope updates without a handler.

func stopGyroUpdates()

Stops gyroscope updates.

var gyroData: CMGyroData?

The latest sample of gyroscope data.

typealias CMGyroHandler

The type of block callback for handling gyroscope data.

### Managing Magnetometer Updates

var magnetometerUpdateInterval: TimeInterval

The interval, in seconds, at which the system delivers magnetometer data to the block handler.

func startMagnetometerUpdates(to: OperationQueue, withHandler: CMMagnetometerHandler)

Starts magnetometer updates on an operation queue and with a specified handler.

func startMagnetometerUpdates()

Starts magnetometer updates without a block handler.

func stopMagnetometerUpdates()

Stops magnetometer updates.

var magnetometerData: CMMagnetometerData?

The latest sample of magnetometer data.

typealias CMMagnetometerHandler

The type of block callback for handling magnetometer data.

### Accessing Attitude Reference Frames

var attitudeReferenceFrame: CMAttitudeReferenceFrame

Returns either the reference frame currently being used or the default attitude reference frame.

class func availableAttitudeReferenceFrames() -> CMAttitudeReferenceFrame

Returns a bitmask of the available reference frames for reporting the attitude of the current device.

### Understanding Errors

let CMErrorDomain: String

The error domain for Core Motion.

struct CMError

Defines motion errors.

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

### Essentials

Core Motion updates

Learn about important changes to Core Motion.

