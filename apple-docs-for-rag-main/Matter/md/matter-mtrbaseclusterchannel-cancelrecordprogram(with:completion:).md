

- Matter
- MTRBaseClusterChannel
-  cancelRecordProgram(with:completion:) 

Instance Method

# cancelRecordProgram(with:completion:)

Command CancelRecordProgram

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func cancelRecordProgram(
    with params: MTRChannelClusterCancelRecordProgramParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func cancelRecordProgram(with params: MTRChannelClusterCancelRecordProgramParams) async throws
```

## Discussion

Cancel recording for a specific program or series.

