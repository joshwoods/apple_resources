

- Video Toolbox
- VTFrameRateConversionConfiguration
-  revision 

Instance Property

# revision

The specific algorithm or configuration revision to use to perform the request.

macOS 15.4+

``` source
var revision: VTFrameRateConversionConfiguration.Revision { get }
```

## See Also

### Inspecting revision information

class var defaultRevision: VTFrameRateConversionConfiguration.Revision

The default revision of a particular algorithm or configuration.

class var supportedRevisions: IndexSet

The collection of currently-supported algorithms or configuration revisions for the class of configurations.

enum Revision

The specific algorithm or configuration revision that is to be used to perform the request.

