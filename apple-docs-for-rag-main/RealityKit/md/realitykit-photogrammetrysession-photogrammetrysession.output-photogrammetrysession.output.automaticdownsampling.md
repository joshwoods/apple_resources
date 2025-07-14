

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.automaticDownsampling 

Case

# PhotogrammetrySession.Output.automaticDownsampling

The session reduced the image size because of memory constraints.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case automaticDownsampling
```

## Discussion

If PhotogrammetrySession encounters serious resource constraints during the object-creation process, it attempts to reduce memory usage by creating scaled-down copies of the sample images, and publishes this message.

## See Also

### Monitoring data ingestion

case invalidSample(id: Int, reason: String)

A provided sample was invalid.

case skippedSample(id: Int)

The type of element used for Object Capture updates. The PhotogrammetrySample with the id indicated was not able to be used for reconstruction.

