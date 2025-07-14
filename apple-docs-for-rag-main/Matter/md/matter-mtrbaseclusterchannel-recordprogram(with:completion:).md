

- Matter
- MTRBaseClusterChannel
-  recordProgram(with:completion:) 

Instance Method

# recordProgram(with:completion:)

Command RecordProgram

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func recordProgram(
    with params: MTRChannelClusterRecordProgramParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func recordProgram(with params: MTRChannelClusterRecordProgramParams) async throws
```

## Discussion

Record a specific program or series when it goes live. This functionality enables DVR recording features.

