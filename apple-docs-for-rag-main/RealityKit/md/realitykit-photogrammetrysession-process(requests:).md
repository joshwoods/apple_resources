

- RealityKit
- PhotogrammetrySession
-  process(requests:) 

Instance Method

# process(requests:)

Starts processing of the provided processing `requests`. Messages begin to be produced to the `output` publisher.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func process(requests: [PhotogrammetrySession.Request]) throws
```

## Mentioned in 

Creating 3D objects from photographs

## Discussion

On the first `process()`call the data in the input source will be ingested entirely and `inputComplete` produced on the `output` stream before any request processing progress will begin. Before `inputComplete`, warnings about samples will be published, if any.

Throws

If `isProcessing` another batch still, the session is invalid (an Error was produced on `output` or if one of the requests is invalid.

## See Also

### Controlling object creation

func cancel()

Requests cancellation of any running requests.

