

- SensorKit
- SRPhotoplethysmogramOpticalSample
-  effectiveWavelength 

Instance Property

# effectiveWavelength

A temperature-compensated wavelength estimate in nanometers that the emitter produces.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var effectiveWavelength: Measurement { get }
```

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

var normalizedReflectance: Double?

The normalized photoplethysmogram (PPG) waveform.

