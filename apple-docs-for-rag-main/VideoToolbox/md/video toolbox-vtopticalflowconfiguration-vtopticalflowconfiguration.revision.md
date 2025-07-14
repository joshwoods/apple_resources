

- Video Toolbox
- VTOpticalFlowConfiguration
-  VTOpticalFlowConfiguration.Revision 

Enumeration

# VTOpticalFlowConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

macOS 15.4+

``` source
enum Revision
```

## Topics

### Enumeration Cases

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

var revision: VTOpticalFlowConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

class var defaultRevision: VTOpticalFlowConfiguration.Revision

The default revision of a particular algorithm or configuration.

class var supportedRevisions: IndexSet

A boolean value that indicates whether the processor supported on the current configuration.

