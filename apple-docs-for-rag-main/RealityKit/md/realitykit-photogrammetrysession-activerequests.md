

- RealityKit
- PhotogrammetrySession
-  activeRequests 

Instance Property

# activeRequests

The session’s active request objects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var activeRequests: [PhotogrammetrySession.Request] { get }
```

## Discussion

This property provides read-only access to the requests that the session actively processes.

## See Also

### Monitoring the session

var isProcessing: Bool

The session is actively processing requests.

var outputs: PhotogrammetrySession.Outputs

Returns the outputs message stream which can be asynchronously iterated on.

enum Output

Status updates on the object-creation process.

