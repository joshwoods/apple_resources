

- Vision
- VNRequest
-  currentRevision 

Type Property

# currentRevision

The current revison supported by the request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class var currentRevision: Int { get }
```

## See Also

### Determining the Revision

protocol VNRequestRevisionProviding

A protocol for specifying the revision number of Vision algorithms.

class var defaultRevision: Int

The revision of the latest request for the particular SDK linked with the client application.

class var supportedRevisions: IndexSet

The collection of currently-supported algorithm versions for the class of request.

