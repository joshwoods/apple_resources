

- CFNetwork
-  CFNetDiagnosticSetName(\_:\_:) Deprecated

Function

# CFNetDiagnosticSetName(\_:\_:)

Overrides the displayed application name.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func CFNetDiagnosticSetName(
    _ details: CFNetDiagnostic,
    _ name: CFString
)
```

## Parameters 

`details`  

The network diagnostics object for which the application name is to be set.

`name`  

Name that is to be set.

## Discussion

Frameworks requiring that an application name be displayed to the user derive the application name from the bundle identifier of the currently running application, in that application’s localization. If you want to override the derived application name, use this function to set the name that is displayed.

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

func CFNetDiagnosticDiagnoseProblemInteractively(CFNetDiagnostic) -> CFNetDiagnosticStatus

Opens a Network Diagnostics window.

Deprecated

