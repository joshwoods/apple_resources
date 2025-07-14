

- Network Extension
- NEFilterDataVerdict
-  init(passBytes:peekBytes:) 

Initializer

# init(passBytes:peekBytes:)

Creates a verdict that tells the system to pass a chunk of network data to its final destination, and specifies the next chunk of data to provide.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
init(
    passBytes: Int,
    peekBytes: Int
)
```

## Parameters 

`passBytes`  

The number of bytes to pass to its final destination.

`peekBytes`  

The number of bytes after the end of the `passBytes` that the Filter Data Provider expects in the next call to handleOutboundData(from:readBytesStartOffset:readBytes:) or handleInboundData(from:readBytesStartOffset:readBytes:). The Filter Data Provider uses this chunk of data to make its next filtering decision.

To see all subsequent bytes, set this parameter to NEFilterFlowBytesMax.

## Return Value

A `NEFilterDataVerdict` object.

## See Also

### Creating data verdicts

class func allow() -> NEFilterDataVerdict

Creates a verdict that tells the system to pass the current chunk of network data and all subsequent data for the current flow to its final destination.

class func drop() -> NEFilterDataVerdict

Creates a verdict that tells the system to drop the current chunk of network data and all subsequent data for the current flow.

class func pause() -> NEFilterDataVerdict

Creates a verdict that tells the system to pause the flow.

class func remediateVerdict(withRemediationURLMapKey: String?, remediationButtonTextMapKey: String?) -> NEFilterDataVerdict

Creates a verdict to drop the current chunk of network data and all subsequent data for the current flow, and provides a remediation URL.

class func needRules() -> NEFilterDataVerdict

Creates a verdict that tells the system that the Filter Control Provider needs to update the rules before making a decision about the flow’s data.

