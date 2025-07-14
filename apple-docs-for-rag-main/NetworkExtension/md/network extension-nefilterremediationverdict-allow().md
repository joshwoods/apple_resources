

- Network Extension
- NEFilterRemediationVerdict
-  allow() 

Type Method

# allow()

Create a verdict that indicates to the system that the Filter Data Provider will allow the flow to pass to its final destination when/if the flow is requested again.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func allow() -> NEFilterRemediationVerdict
```

## Return Value

A `NEFilterRemediationVerdict` object.

## See Also

### Creating remediation verdicts

class func drop() -> NEFilterRemediationVerdict

Create a verdict that indicates to the system that the Filter Data Provider will continue to block the flow of network data if/when the flow is requested again.

class func needRules() -> NEFilterRemediationVerdict

Create a verdict that indicates to the system that the Filter Data Provider needs the filtering rules to be updated before it can make a remediation decision about the current flow of network data.

