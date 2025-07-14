

- GameplayKit
- GKCoherentNoiseSource
-  octaveCount 

Instance Property

# octaveCount

The number of octaves of the underlying noise function to use for generating noise.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var octaveCount: Int { get set }
```

## Discussion

Coherent noise is composed from several applications of a pseudorandom function. Each successive application, or *octave*, increases in frequency and decreases in amplitude relative to the previous octave. This combination of many octaves produces the fractal appearance that makes coherent noise resemble natural phenomena like clouds, stone, and water.

This property determines the number of octaves of the noise function that the noise source combines to produce noise. A smaller number results in smoother, simpler output; larger numbers result in rougher, more complex output. The default value is `6`.

## See Also

### Managing Noise Generation Parameters

var frequency: Double

A value that determines the size and spacing of features in generated noise.

var lacunarity: Double

The rate at which successive octaves of the noise function increase in frequency.

var seed: Int32

The value that determines the specific configuration of noise produced by the noise source.

