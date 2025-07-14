

- Accelerate
- vDSP
- vDSP.DFT
-  init(previous:count:direction:transformType:ofType:) Deprecated

Initializer

# init(previous:count:direction:transformType:ofType:)

Initializes a new discrete Fourier transform instance.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init?(
    previous: vDSP.DFT? = nil,
    count: Int,
    direction: vDSP.FourierTransformDirection,
    transformType: vDSP.DFTTransformType,
    ofType: T.Type
)
```

Deprecated

Use `vDSP.DiscreteFourierTransform`.

