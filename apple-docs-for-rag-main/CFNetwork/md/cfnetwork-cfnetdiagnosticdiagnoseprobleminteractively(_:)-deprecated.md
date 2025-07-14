

- CFNetwork
-  CFNetDiagnosticDiagnoseProblemInteractively(\_:) Deprecated

Function

# CFNetDiagnosticDiagnoseProblemInteractively(\_:)

Opens a Network Diagnostics window.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func CFNetDiagnosticDiagnoseProblemInteractively(_ details: CFNetDiagnostic) -> CFNetDiagnosticStatus
```

## Parameters 

`details`  

A network diagnostics object, created by CFNetDiagnosticCreateWithStreams(_:_:_:) or CFNetDiagnosticCreateWithURL(_:_:), for which the window is to be opened.

## Return Value

`CFNetDiagnosticNoErr` if no error occurred, or `CFNetDiagnosticErr` if an error occurred that prevented this call from completing successfully.

## Discussion

This function opens the Network Diagnostics window and returns immediately once the window is open.

### Special Considerations

This function is thread safe as long as another thread does not alter the same CFNetDiagnosticRef at the same time.

## See Also

### Network Diagnostics

class CFNetDiagnostic

An opaque reference representing a CFNetDiagnostic.

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

func CFNetDiagnosticSetName(CFNetDiagnostic, CFString)

Overrides the displayed application name.

Deprecated

