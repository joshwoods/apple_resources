

- Core Motion
-  CMBatchedSensorManager 

Class

# CMBatchedSensorManager

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
class CMBatchedSensorManager
```

## Mentioned in 

Getting processed device-motion data

## Topics

### Determining authorization and availability

class var authorizationStatus: CMAuthorizationStatus

class var isAccelerometerSupported: Bool

class var isDeviceMotionSupported: Bool

### Configuring the update frequency

var deviceMotionDataFrequency: Int

var accelerometerDataFrequency: Int

### Collecting device-motion data

func startDeviceMotionUpdates()

func startDeviceMotionUpdates(handler: ([CMDeviceMotion]?, (any Error)?) -> Void)

func stopDeviceMotionUpdates()

var deviceMotionBatch: [CMDeviceMotion]?

func deviceMotionUpdates() -> CMBatchedSensorManager.DeviceMotionUpdates

struct DeviceMotionUpdates

var isDeviceMotionActive: Bool

### Collecting accelerometer data

func startAccelerometerUpdates()

func startAccelerometerUpdates(handler: ([CMAccelerometerData]?, (any Error)?) -> Void)

func stopAccelerometerUpdates()

var accelerometerBatch: [CMAccelerometerData]?

func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates

struct AccelerometerUpdates

var isAccelerometerActive: Bool

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

