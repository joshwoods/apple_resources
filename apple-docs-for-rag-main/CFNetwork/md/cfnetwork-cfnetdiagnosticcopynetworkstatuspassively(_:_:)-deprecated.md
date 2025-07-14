

- CFNetwork
-  CFNetDiagnosticCopyNetworkStatusPassively(\_:\_:) Deprecated

Function

# CFNetDiagnosticCopyNetworkStatusPassively(\_:\_:)

Gets a network status value.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func CFNetDiagnosticCopyNetworkStatusPassively(
    _ details: CFNetDiagnostic,
    _ description: UnsafeMutablePointer?>?
) -> CFNetDiagnosticStatus
```

## Parameters 

`details`  

CFNetDiagnosticRef, created by CFNetDiagnosticCreateWithStreams(_:_:_:) or CFNetDiagnosticCreateWithURL(_:_:), for which the Network Diagnostics status is to be obtained.

`description`  

If not `NULL`, upon return contains a localized string containing a description of the current network status. Ownership follows the The Create Rule.

## Return Value

A network status value.

## Discussion

This function returns a status value that can be used to display basic information about the connection, and optionally gets a localized string containing a description of the current network status.

This function is guaranteed not to generate network activity.

### Special Considerations

This function is thread safe as long as another thread does not alter the same CFNetDiagnosticRef at the same time.

## See Also

### Network Diagnostics

class CFNetDiagnostic

An opaque reference representing a CFNetDiagnostic.

enum CFNetDiagnosticStatusValues

Constants for diagnostic status values.

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

