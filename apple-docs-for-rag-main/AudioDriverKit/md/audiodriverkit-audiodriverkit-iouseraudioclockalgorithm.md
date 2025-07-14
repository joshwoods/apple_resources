

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioClockAlgorithm 

Enumeration

# IOUserAudioClockAlgorithm

Values that describe clock-smoothing algorithms.

DriverKit 21.0+

``` source
enum IOUserAudioClockAlgorithm : uint32_t;
```

## Topics

### Clock-Smoothing Algorithms

Raw

An algorithm that uses timestamp values as-is.

SimpleIIR

The simple IIR filter algorithm.

TwelvePtMovingWindowAverage

The 12-point moving window average filter algorithm.

## See Also

### Working with Clock Device Behavior

SetClockAlgorithm

Sets the clock algorithm of the clock device.

GetClockAlgorithm

Gets the clock algorithm of the clock device.

SetClockIsStable

Sets a Boolean value to represent the clock’s stability.

GetClockIsStable

Gets a Boolean value that represents the clock’s stability.

