

- RealityKit
- PhotogrammetrySession
-  outputs 

Instance Property

# outputs

Returns the outputs message stream which can be asynchronously iterated on.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var outputs: PhotogrammetrySession.Outputs { get }
```

## Mentioned in 

Creating 3D objects from photographs

## See Also

### Monitoring the session

var activeRequests: [PhotogrammetrySession.Request]

The session’s active request objects.

var isProcessing: Bool

The session is actively processing requests.

enum Output

Status updates on the object-creation process.

