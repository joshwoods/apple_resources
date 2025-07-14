

- SensorKit
-  SRSensorReader 

Class

# SRSensorReader

An object that establishes user authorization and records data for a particular sensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRSensorReader
```

## Overview

To acquire data from a particular sensor using a reader, an app creates an instance of this class using init(sensor:) and passes in one sensor from the available options in `Sensors`.

A reader is a data stream for a particular sensor that the user must authorize before use. When an app calls requestAuthorization(sensors:completion:), the OS prompts the user for approval to use the particular sensor and determines the app’s authorization according to the user’s answer. The framework notifies the delegate with the sensorReader(_:didChange:) callback if the authorization status changes as a result of the requestAuthorization(sensors:completion:) call. When a reader’s authorizationStatus is SRAuthorizationStatus.authorized, an app starts collecting sensor data by beginning recording.

When an app calls startRecording(), the framework starts the reader’s sensor if it isn’t already running because of a request from another app or a system process. An app has access to 7 days of prior recorded data for an active sensor. When an app calls stopRecording(), the app relinquishes stakeholdership in the sensor. When a sensor has no app or system stakeholders, the framework deactivates the sensor and, thereby, stops recording data.

To fetch a sensor’s data, pass a request object to the fetch(_:) function. SRFetchRequest specifies a time range that defines the age of the data, and a device, such as a phone or a watch, from which to collect the data. Use fetchDevices() to list the available devices, and use the time convenience-functions in Defining the Time Range to specify the time range.

If the fetch query succeeds, the framework notifies the delegate with sensorReader(_:didCompleteFetch:). The delegate receives sensor data in the form of *samples* from sensorReader(_:fetching:didFetchResult:). A fetch result’s sample type is different depending on the particular sensor for the reader. For a mapping of sensors to their samples, see Sample types.

## Topics

### Checking user authorization

var authorizationStatus: SRAuthorizationStatus

The status of the user’s agreement to let the app access this reader’s sensor.

class func requestAuthorization(sensors: Set&lt;SRSensor>, completion: ((any Error)?) -> Void)

Requests user permission to read one or more sensors.

enum SRAuthorizationStatus

The states that model whether the user approves the app to read a particular sensor.

### Creating a sensor reader

init(sensor: SRSensor)

Initializes a new sensor reader object.

struct SRSensor

The sensors an app can read.

var sensor: SRSensor

The particular sensor that this object reads.

### Recording sensor data

func startRecording()

Starts recording sensor data.

func stopRecording()

Stops recording sensor data.

### Reading recorded data

func fetch(SRFetchRequest)

Fetches the samples that a fetch request specifies.

func fetchDevices()

Acquires device information for all devices that store data for this reader’s sensor.

class SRDevice

A representation of a device that provides sample data.

### Responding to sensor events

var delegate: (any SRSensorReaderDelegate)?

An object that responds to sensor-related events.

protocol SRSensorReaderDelegate

A set of callbacks the framework invokes to notify the app of sensor-related events.

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

### Setup

Configuring your project for sensor reading

Add metadata to your app to attain system and user permission to access sensor data.

