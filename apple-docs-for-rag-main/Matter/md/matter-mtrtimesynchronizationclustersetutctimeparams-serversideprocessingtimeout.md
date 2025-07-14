

- Matter
- MTRTimeSynchronizationClusterSetUTCTimeParams
-  serverSideProcessingTimeout 

Instance Property

# serverSideProcessingTimeout

Controls how much time, in seconds, we will allow for the server to process the command.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
@NSCopying
var serverSideProcessingTimeout: NSNumber? { get set }
```

## Discussion

The command will then time out if that much time, plus an allowance for retransmits due to network failures, passes.

If nil, the framework will try to select an appropriate timeout value itself.

