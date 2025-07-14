

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClockAlgorithm
-  TwelvePtMovingWindowAverage 

Enumeration Case

# TwelvePtMovingWindowAverage

The 12-point moving window average filter algorithm.

DriverKit 21.0+

``` source
TwelvePtMovingWindowAverage
```

## Discussion

Under this algorithm, the Host applies 12 point moving window average filter to the time stamps returned from GetCurrentZeroTimestamp.

## See Also

### Clock-Smoothing Algorithms

Raw

An algorithm that uses timestamp values as-is.

SimpleIIR

The simple IIR filter algorithm.

