

- CFNetwork
-  CFNetDiagnostic 

Class

# CFNetDiagnostic

An opaque reference representing a CFNetDiagnostic.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class CFNetDiagnostic
```

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Network Diagnostics

enum CFNetDiagnosticStatusValues

Constants for diagnostic status values.

Deprecated

func CFNetDiagnosticCopyNetworkStatusPassively(CFNetDiagnostic, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>?) -> CFNetDiagnosticStatus

Gets a network status value.

Deprecated

func CFNetDiagnosticCreateWithStreams(CFAllocator?, CFReadStream?, CFWriteStream?) -> Unmanaged&lt;CFNetDiagnostic>

Creates a network diagnostic object from a pair of CFStreams.

Deprecated

func CFNetDiagnosticCreateWithURL(CFAllocator, CFURL) -> Unmanaged&lt;CFNetDiagnostic>

Creates a CFNetDiagnosticRef from a CFURLRef.

Deprecated

func CFNetDiagnosticDiagnoseProblemInteractively(CFNetDiagnostic) -> CFNetDiagnosticStatus

Opens a Network Diagnostics window.

Deprecated

func CFNetDiagnosticSetName(CFNetDiagnostic, CFString)

Overrides the displayed application name.

Deprecated

