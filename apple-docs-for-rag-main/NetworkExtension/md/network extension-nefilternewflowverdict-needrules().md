

- Network Extension
- NEFilterNewFlowVerdict
-  needRules() 

Type Method

# needRules()

Create a verdict that indicates to the system that the Filter Data Provider needs more information before it can make a decision about a new flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func needRules() -> NEFilterNewFlowVerdict
```

## Return Value

A `NEFilterNewFlowVerdict` object.

## Discussion

When the Filter Data Provider returns this object from its `handleNewFlow:` method, the system calls the Filter Control Provider’s handleNewFlow(_:completionHandler:) method.

## See Also

### Creating new flow verdicts

class func allow() -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that the all of the new flow’s data should be allowed to pass to its final destination.

class func drop() -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that all of the new flow’s data should dropped, and the user should not be given the opportunity to request access.

class func pause() -> NEFilterNewFlowVerdict

Creates a verdict that tells the system to pause the flow.

class func filterDataVerdict(withFilterInbound: Bool, peekInboundBytes: Int, filterOutbound: Bool, peekOutboundBytes: Int) -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that the filter needs to make a decision about a new flow after seeing a portion of the flow’s data.

class func remediateVerdict(withRemediationURLMapKey: String, remediationButtonTextMapKey: String) -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that all of the new flow’s data should be dropped, but allow the user to request access by tapping or clicking on a URL.

class func urlAppendStringVerdict(withMapKey: String) -> NEFilterNewFlowVerdict

Create a verdict that indicates to the system that all of the new flow’s data should be allowed to pass to its final destination, but a string should first be appended to the new flow’s request URL.

