

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClockAlgorithm
-  SimpleIIR 

Enumeration Case

# SimpleIIR

The simple IIR filter algorithm.

DriverKit 21.0+

``` source
SimpleIIR
```

## Discussion

Under this algorithm, the Host applies a simple IIR filter to the time stamp stream. This is the default algorithm used for devices that don’t implement `DevicePropertyClockAlgorithm`.

## See Also

### Clock-Smoothing Algorithms

Raw

An algorithm that uses timestamp values as-is.

TwelvePtMovingWindowAverage

The 12-point moving window average filter algorithm.

