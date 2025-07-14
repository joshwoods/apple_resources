

- SensorKit
- SRPhotoplethysmogramOpticalSample
-  SRPhotoplethysmogramOpticalSample.NoiseTerms 

Structure

# SRPhotoplethysmogramOpticalSample.NoiseTerms

The mathematical terms that you use to compute the photoplethysmogram (PPG) noise.

iOS 17.4+iPadOS 17.4+

``` source
struct NoiseTerms
```

## Overview

To estimate the total ambient noise, subtract the scaled background noise offset (backgroundNoiseOffset) from the background noise (backgroundNoise). Compute the scaling factor (normalized noise equivalent bandwidth) based on your digital filter setup.

## Topics

### Accessing noise terms

let whiteNoise: Double

An estimate of the white noise of the sensor.

let pinkNoise: Double

An estimate of the pink noise of the sensor.

let backgroundNoise: Double

An estimate of the ambient noise intrusion of the sensor.

let backgroundNoiseOffset: Double

An estimate of the electronics noise floor level of the sensor.

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

var normalizedReflectance: Double?

The normalized photoplethysmogram (PPG) waveform.

