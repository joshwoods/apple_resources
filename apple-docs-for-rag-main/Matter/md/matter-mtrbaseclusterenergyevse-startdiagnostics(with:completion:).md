

- Matter
- MTRBaseClusterEnergyEVSE
-  startDiagnostics(with:completion:) 

Instance Method

# startDiagnostics(with:completion:)

Command StartDiagnostics

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func startDiagnostics(
    with params: MTREnergyEVSEClusterStartDiagnosticsParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func startDiagnostics(with params: MTREnergyEVSEClusterStartDiagnosticsParams?) async throws
```

## Discussion

Allows a client to put the EVSE into a self-diagnostics mode.

