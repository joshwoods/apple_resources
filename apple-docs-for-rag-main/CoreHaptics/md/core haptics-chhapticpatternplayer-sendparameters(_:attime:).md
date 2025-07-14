

- Core Haptics
- CHHapticPatternPlayer
-  sendParameters(\_:atTime:) 

Instance Method

# sendParameters(\_:atTime:)

Sends an array of haptic parameters, starting at the specified time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func sendParameters(
    _ parameters: [CHHapticDynamicParameter],
    atTime time: TimeInterval
) throws
```

**Required**

## Parameters 

`parameters`  

An array of dynamic parameters to send together.

`time`  

The time at which to send the dynamic parameters.

## Discussion

If `time` is `0` or any value less than the haptic engine’s currentTime, this method sends parameters immediately.

## See Also

### Sending Parameters to a Haptic

func scheduleParameterCurve(CHHapticParameterCurve, atTime: TimeInterval) throws

Schedules a parameter curve to begin transitioning a parameter at a certain time.

**Required**

