

- Video Toolbox
- VTMotionBlurConfiguration
-  VTMotionBlurConfiguration.Revision 

Enumeration

# VTMotionBlurConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

macOS 15.4+

``` source
enum Revision
```

## Topics

### Revisions

case revision1

An algorithm or implementation that represents the first revision.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting revision information

var revision: VTMotionBlurConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

class var defaultRevision: VTMotionBlurConfiguration.Revision

The default revision of a particular algorithm or configuration.

class var supportedRevisions: IndexSet

The collection of currently-supported algorithms or configuration revisions for the class of configurations.

