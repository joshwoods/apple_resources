

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Output
-  PhotogrammetrySession.Output.inputComplete 

Case

# PhotogrammetrySession.Output.inputComplete

The data ingestion portion of the process is complete.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case inputComplete
```

## Discussion

Once the session sends this messagae, processing on the actual requests begins. It only sends this on the first `process()` call after which the data from the original processing is reused.

## See Also

### Monitoring session status

case processingComplete

The session completed a request successfully.

case processingCancelled

All pending requests are canceled.

