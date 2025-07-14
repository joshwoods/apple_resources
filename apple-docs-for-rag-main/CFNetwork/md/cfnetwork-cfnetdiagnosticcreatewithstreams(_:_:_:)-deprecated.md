

- CFNetwork
-  CFNetDiagnosticCreateWithStreams(\_:\_:\_:) Deprecated

Function

# CFNetDiagnosticCreateWithStreams(\_:\_:\_:)

Creates a network diagnostic object from a pair of CFStreams.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func CFNetDiagnosticCreateWithStreams(
    _ alloc: CFAllocator?,
    _ readStream: CFReadStream?,
    _ writeStream: CFWriteStream?
) -> Unmanaged
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`readStream`  

Reference to a read stream whose connection has failed, or `NULL` if you do not want the CFNetDiagnosticRef to have a read stream.

`writeStream`  

Reference to a write stream whose connection has failed, or `NULL` if you do not want the CFNetDiagnosticRef to have a write stream.

## Discussion

This function uses references to a read steam and a write stream (or just a read stream or just a write stream) to create a reference to an instance of a CFNetDiagnostic object. You can pass the reference to CFNetDiagnosticDiagnoseProblemInteractively(_:) to open a Network Diagnostics window or to CFNetDiagnosticCopyNetworkStatusPassively(_:_:) to get a description of the connection referenced by `readStream` and `writeStream`.

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

func CFNetDiagnosticCreateWithURL(CFAllocator, CFURL) -> Unmanaged&lt;CFNetDiagnostic>

Creates a CFNetDiagnosticRef from a CFURLRef.

Deprecated

func CFNetDiagnosticDiagnoseProblemInteractively(CFNetDiagnostic) -> CFNetDiagnosticStatus

Opens a Network Diagnostics window.

Deprecated

func CFNetDiagnosticSetName(CFNetDiagnostic, CFString)

Overrides the displayed application name.

Deprecated

