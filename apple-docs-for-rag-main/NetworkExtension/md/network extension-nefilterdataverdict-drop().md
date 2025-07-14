

- Network Extension
- NEFilterDataVerdict
-  drop() 

Type Method

# drop()

Creates a verdict that tells the system to drop the current chunk of network data and all subsequent data for the current flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class func drop() -> NEFilterDataVerdict
```

## Return Value

A `NEFilterDataVerdict` object.

## See Also

### Creating data verdicts

class func allow() -> NEFilterDataVerdict

Creates a verdict that tells the system to pass the current chunk of network data and all subsequent data for the current flow to its final destination.

class func pause() -> NEFilterDataVerdict

Creates a verdict that tells the system to pause the flow.

class func remediateVerdict(withRemediationURLMapKey: String?, remediationButtonTextMapKey: String?) -> NEFilterDataVerdict

Creates a verdict to drop the current chunk of network data and all subsequent data for the current flow, and provides a remediation URL.

class func needRules() -> NEFilterDataVerdict

Creates a verdict that tells the system that the Filter Control Provider needs to update the rules before making a decision about the flow’s data.

init(passBytes: Int, peekBytes: Int)

Creates a verdict that tells the system to pass a chunk of network data to its final destination, and specifies the next chunk of data to provide.

