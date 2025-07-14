

- Video Toolbox
- VTMotionBlurConfiguration
-  supportedRevisions 

Type Property

# supportedRevisions

The collection of currently-supported algorithms or configuration revisions for the class of configurations.

macOS 15.4+

``` source
class var supportedRevisions: IndexSet { get }
```

## Discussion

This property allows you to check what revisions are available for each configuration at runtime.

## See Also

### Inspecting revision information

var revision: VTMotionBlurConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

class var defaultRevision: VTMotionBlurConfiguration.Revision

The default revision of a particular algorithm or configuration.

enum Revision

The specific algorithm or configuration revision that is to be used to perform the request.

