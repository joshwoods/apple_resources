

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.invalidSample(id:reason:) 

Case

# PhotogrammetrySession.Output.invalidSample(id:reason:)

A provided sample was invalid.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case invalidSample(
    id: Int,
    reason: String
)
```

## Parameters 

`id`  

The sample ID.

`reason`  

The reason the sample is invalid.

## See Also

### Monitoring data ingestion

case automaticDownsampling

The session reduced the image size because of memory constraints.

case skippedSample(id: Int)

The type of element used for Object Capture updates. The PhotogrammetrySample with the id indicated was not able to be used for reconstruction.

