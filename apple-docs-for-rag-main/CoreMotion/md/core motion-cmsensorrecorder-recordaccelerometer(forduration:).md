

- Core Motion
- CMSensorRecorder
-  recordAccelerometer(forDuration:) 

Instance Method

# recordAccelerometer(forDuration:)

Begins recording accelerometer data for the specified period of time.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func recordAccelerometer(forDuration duration: TimeInterval)
```

## Parameters 

`duration`  

The amount of time (in seconds) for which to record the data. You may specify a time interval of up to 43,200 seconds (12 hours).

## Discussion

When you call this method, the system begins capturing accelerometer data at a sample rate of 50 Hz. The system records the data for the specified amount of time, even if your app is suspended or terminated. The collected data remains accessible to your app for up to three days.

