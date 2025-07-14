

- RealityKit
- PhotogrammetrySession
-  isProcessing 

Instance Property

# isProcessing

The session is actively processing requests.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var isProcessing: Bool { get }
```

## See Also

### Monitoring the session

var activeRequests: [PhotogrammetrySession.Request]

The session’s active request objects.

var outputs: PhotogrammetrySession.Outputs

Returns the outputs message stream which can be asynchronously iterated on.

enum Output

Status updates on the object-creation process.

