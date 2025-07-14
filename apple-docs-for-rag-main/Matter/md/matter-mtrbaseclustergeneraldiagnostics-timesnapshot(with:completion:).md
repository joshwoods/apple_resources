

- Matter
- MTRBaseClusterGeneralDiagnostics
-  timeSnapshot(with:completion:) 

Instance Method

# timeSnapshot(with:completion:)

Command TimeSnapshot

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func timeSnapshot(
    with params: MTRGeneralDiagnosticsClusterTimeSnapshotParams?,
    completion: @escaping (MTRGeneralDiagnosticsClusterTimeSnapshotResponseParams?, (any Error)?) -> Void
)
```

``` source
func timeSnapshot(with params: MTRGeneralDiagnosticsClusterTimeSnapshotParams?) async throws -> MTRGeneralDiagnosticsClusterTimeSnapshotResponseParams
```

## Discussion

Take a snapshot of system time and epoch time.

