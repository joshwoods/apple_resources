

- CFNetwork
-  CFNetDiagnosticStatusValues Deprecated

Enumeration

# CFNetDiagnosticStatusValues

Constants for diagnostic status values.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum CFNetDiagnosticStatusValues
```

## Overview

Diagnostic status values are returned by CFNetDiagnosticDiagnoseProblemInteractively(_:) and CFNetDiagnosticCopyNetworkStatusPassively(_:_:).

## Topics

### Constants

case noErr

No error occurred but there is no status.

case err

An error occurred that prevented the call from completing.

case connectionUp

The connection appears to be working.

case connectionIndeterminate

The status of the connection is not known.

case connectionDown

The connection does not appear to be working.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Network Diagnostics

class CFNetDiagnostic

An opaque reference representing a CFNetDiagnostic.

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

