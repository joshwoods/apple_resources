

- Video Toolbox
- VTFrameRateConversionConfiguration
-  supportedRevisions 

Type Property

# supportedRevisions

The collection of currently-supported algorithms or configuration revisions for the class of configurations.

macOS 15.4+

``` source
class var supportedRevisions: IndexSet { get }
```

## Discussion

Use this property to determine the supported revisions for each configuration at runtime.

## See Also

### Inspecting revision information

var revision: VTFrameRateConversionConfiguration.Revision

The specific algorithm or configuration revision to use to perform the request.

class var defaultRevision: VTFrameRateConversionConfiguration.Revision

The default revision of a particular algorithm or configuration.

enum Revision

The specific algorithm or configuration revision that is to be used to perform the request.

