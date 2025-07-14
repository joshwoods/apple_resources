

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.skippedSample(id:) 

Case

# PhotogrammetrySession.Output.skippedSample(id:)

The type of element used for Object Capture updates. The PhotogrammetrySample with the id indicated was not able to be used for reconstruction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case skippedSample(id: Int)
```

## See Also

### Monitoring data ingestion

case invalidSample(id: Int, reason: String)

A provided sample was invalid.

case automaticDownsampling

The session reduced the image size because of memory constraints.

