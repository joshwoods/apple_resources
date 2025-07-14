

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClockAlgorithm
-  Raw 

Enumeration Case

# Raw

An algorithm that uses timestamp values as-is.

DriverKit 21.0+

``` source
Raw
```

## Discussion

Under this algorithm, the Host doesn’t apply any filtering to the time stamps returned from GetCurrentZeroTimestamp.

## See Also

### Clock-Smoothing Algorithms

SimpleIIR

The simple IIR filter algorithm.

TwelvePtMovingWindowAverage

The 12-point moving window average filter algorithm.

