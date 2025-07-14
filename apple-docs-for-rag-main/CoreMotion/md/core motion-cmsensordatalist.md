

- Core Motion
-  CMSensorDataList 

Class

# CMSensorDataList

A list of the accelerometer data recorded by the system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
class CMSensorDataList
```

## Overview

You do not create instances of this class directly. Instead, you receive one as the result of a query for accelerometer data from a CMSensorRecorder object.

You use a sensor data list object to enumerate over the accelerometer data as shown in the following example:

```
-(void)processSamplesFromDate:(NSDate*)start toDate:(NSDate)end {
   CMSensorRecorder* recorder = [[CMSensorRecorder alloc] init];
   CMSensorDataList* list = [recorder accelerometerDataFrom:start to:end];

   for (CMRecordedAccelerometerData* data in list) {
      // Process the data.
      NSLog(@"Sample: (%f, %f, %f)", data.acceleration.x,
              data.acceleration.y, data.acceleration.z);
   }
}
```

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSFastEnumeration
- NSObjectProtocol

## See Also

### Accelerometers

Getting raw accelerometer events

Retrieve data from the onboard accelerometers.

class CMAccelerometerData

A data sample from the device’s three accelerometers.

class CMRecordedAccelerometerData

A single piece of accelerometer data that was recorded by the device.

class CMSensorRecorder

An object that gathers and retrieves accelerometer data from a device.

