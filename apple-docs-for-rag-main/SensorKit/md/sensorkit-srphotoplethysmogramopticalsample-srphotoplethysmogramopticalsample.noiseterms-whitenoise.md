

- SensorKit
- SRPhotoplethysmogramOpticalSample
- SRPhotoplethysmogramOpticalSample.NoiseTerms
-  whiteNoise 

Instance Property

# whiteNoise

An estimate of the white noise of the sensor.

iOS 17.4+iPadOS 17.4+

``` source
let whiteNoise: Double
```

## Discussion

To account for in-band noise for your setup, apply the normalized noise equivalent bandwidth factor.

## See Also

### Accessing noise terms

let pinkNoise: Double

An estimate of the pink noise of the sensor.

let backgroundNoise: Double

An estimate of the ambient noise intrusion of the sensor.

let backgroundNoiseOffset: Double

An estimate of the electronics noise floor level of the sensor.

