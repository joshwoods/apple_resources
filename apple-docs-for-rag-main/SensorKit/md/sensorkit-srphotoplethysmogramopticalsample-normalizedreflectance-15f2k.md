

- SensorKit
- SRPhotoplethysmogramOpticalSample
-  normalizedReflectance 

Instance Property

# normalizedReflectance

The normalized photoplethysmogram (PPG) waveform.

iOS 17.4+iPadOS 17.4+

``` source
var normalizedReflectance: Double? { get }
```

## Discussion

If the sensor data is invalid, this property is nil.

## See Also

### Accessing optical data

var emitter: Int

The index of the LED in use during the sample.

var activePhotodiodeIndexes: IndexSet

The set of photodiodes in use during the sample.

var signalIdentifier: Int

The identifier for a signal that photodiodes and emitters produce.

var nominalWavelength: Measurement&lt;UnitLength>

The wavelength in nanometers that the emitter produces while operating at a specific temperature.

var effectiveWavelength: Measurement&lt;UnitLength>

A temperature-compensated wavelength estimate in nanometers that the emitter produces.

var samplingFrequency: Measurement&lt;UnitFrequency>

The sampling frequency of the photoplethysmogram (PPG) data in hertz.

var nanosecondsSinceStart: Int64

The time in nanoseconds since the system turns on the sensor.

var conditions: [SRPhotoplethysmogramOpticalSample.Condition]

The sensor context or conditions that may affect the sample.

struct Condition

The conditions that may occur when recording photoplethysmogram optical data.

var noiseTerms: SRPhotoplethysmogramOpticalSample.NoiseTerms?

The mathematical terms for computing the noise in this sample.

struct NoiseTerms

The mathematical terms that you use to compute the photoplethysmogram (PPG) noise.

