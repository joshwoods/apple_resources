

- SensorKit
-  SRSensorReaderDelegate 

Protocol

# SRSensorReaderDelegate

A set of callbacks the framework invokes to notify the app of sensor-related events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
protocol SRSensorReaderDelegate : NSObjectProtocol
```

## Overview

To access sensor data, assign an object as the delegate and implement its callbacks.

## Topics

### Checking Authorization Status

func sensorReader(SRSensorReader, didChange: SRAuthorizationStatus)

Notifies the delegate of the reader’s new authorization status.

### Fetching Devices

func sensorReader(SRSensorReader, didFetch: [SRDevice])

Provides the delegate with one or more devices.

func sensorReader(SRSensorReader, fetchDevicesDidFailWithError: any Error)

Provides the delegate a reason when the reader fails to fetch devices.

class SRDevice

A representation of a device that provides sample data.

### Recording Data

func sensorReaderWillStartRecording(SRSensorReader)

Notifies the delegate when a reader starts recording.

func sensorReader(SRSensorReader, startRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to record.

func sensorReaderDidStopRecording(SRSensorReader)

Notifies the delegate when a reader stops recording.

func sensorReader(SRSensorReader, stopRecordingFailedWithError: any Error)

Provides the delegate with a reason when the reader fails to stop recording.

### Reading Recorded Data

func sensorReader(SRSensorReader, fetching: SRFetchRequest, didFetchResult: SRFetchResult&lt;AnyObject>) -> Bool

Provides the delegate with a fetch result.

func sensorReader(SRSensorReader, didCompleteFetch: SRFetchRequest)

Provides the delegate with a completed fetch request.

func sensorReader(SRSensorReader, fetching: SRFetchRequest, failedWithError: any Error)

Provides the delegate with a fetch failure reason.

### Interpreting Errors

let SRErrorDomain: String

An error domain that’s unique to the framework.

struct SRError

An error that SensorKit reports.

enum Code

The kinds of problems that stop a recording or a fetch.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to sensor events

var delegate: (any SRSensorReaderDelegate)?

An object that responds to sensor-related events.

