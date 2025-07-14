

- Video Toolbox
- VTOpticalFlowConfiguration
-  supportedRevisions 

Type Property

# supportedRevisions

A boolean value that indicates whether the processor supported on the current configuration.

macOS 15.4+

``` source
class var supportedRevisions: IndexSet { get }
```

## See Also

### Inspecting revision information

var revision: VTOpticalFlowConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

class var defaultRevision: VTOpticalFlowConfiguration.Revision

The default revision of a particular algorithm or configuration.

enum Revision

The specific algorithm or configuration revision that is to be used to perform the request.

