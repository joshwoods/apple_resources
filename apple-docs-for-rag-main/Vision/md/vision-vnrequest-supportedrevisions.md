

- Vision
- VNRequest
-  supportedRevisions 

Type Property

# supportedRevisions

The collection of currently-supported algorithm versions for the class of request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class var supportedRevisions: IndexSet { get }
```

## Discussion

This method allows clients to inspect at runtime what capabilities are available for each class of VNRequest in the Vision framework.

## See Also

### Determining the Revision

protocol VNRequestRevisionProviding

A protocol for specifying the revision number of Vision algorithms.

class var currentRevision: Int

The current revison supported by the request.

class var defaultRevision: Int

The revision of the latest request for the particular SDK linked with the client application.

