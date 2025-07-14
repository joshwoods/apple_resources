

- Matter
- MTRBaseClusterGeneralDiagnostics
-  payloadTestRequest(with:completion:) 

Instance Method

# payloadTestRequest(with:completion:)

Command PayloadTestRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func payloadTestRequest(
    with params: MTRGeneralDiagnosticsClusterPayloadTestRequestParams,
    completion: @escaping (MTRGeneralDiagnosticsClusterPayloadTestResponseParams?, (any Error)?) -> Void
)
```

``` source
func payloadTestRequest(with params: MTRGeneralDiagnosticsClusterPayloadTestRequestParams) async throws -> MTRGeneralDiagnosticsClusterPayloadTestResponseParams
```

## Discussion

Request a variable length payload response.

