

- Video Toolbox
- VTFrameRateConversionConfiguration
-  defaultRevision 

Type Property

# defaultRevision

The default revision of a particular algorithm or configuration.

macOS 15.4+

``` source
class var defaultRevision: VTFrameRateConversionConfiguration.Revision { get }
```

## See Also

### Inspecting revision information

var revision: VTFrameRateConversionConfiguration.Revision

The specific algorithm or configuration revision to use to perform the request.

class var supportedRevisions: IndexSet

The collection of currently-supported algorithms or configuration revisions for the class of configurations.

enum Revision

The specific algorithm or configuration revision that is to be used to perform the request.

