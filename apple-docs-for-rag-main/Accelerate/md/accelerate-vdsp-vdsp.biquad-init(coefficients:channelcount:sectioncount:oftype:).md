

- Accelerate
- vDSP
- vDSP.Biquad
-  init(coefficients:channelCount:sectionCount:ofType:) 

Initializer

# init(coefficients:channelCount:sectionCount:ofType:)

Creates a new single-channel or multichannel cascaded biquad IIR structure.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init?(
    coefficients: [Double],
    channelCount: vDSP_Length,
    sectionCount: vDSP_Length,
    ofType: T.Type
)
```

