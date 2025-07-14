

- Network Extension
-  NEFilterRemediationVerdict 

Class

# NEFilterRemediationVerdict

The result from a filter data provider after the user requests remediation for a blocked flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEFilterRemediationVerdict
```

## Topics

### Creating remediation verdicts

class func allow() -> NEFilterRemediationVerdict

Create a verdict that indicates to the system that the Filter Data Provider will allow the flow to pass to its final destination when/if the flow is requested again.

class func drop() -> NEFilterRemediationVerdict

Create a verdict that indicates to the system that the Filter Data Provider will continue to block the flow of network data if/when the flow is requested again.

class func needRules() -> NEFilterRemediationVerdict

Create a verdict that indicates to the system that the Filter Data Provider needs the filtering rules to be updated before it can make a remediation decision about the current flow of network data.

## Relationships

### Inherits From

- NEFilterVerdict

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Flow handling

class NEFilterFlow

The abstract base class for types that represent flows of network data.

class NEFilterBrowserFlow

A flow of network data, originating from a WebKit-based browser, that the filter examines.

class NEFilterSocketFlow

A flow of network data that the filter examines.

class NEFilterNewFlowVerdict

The result from a filter data provder after the initial examination of a flow.

class NEFilterDataVerdict

The result from a filter data provder for subsequent chunks of data on a flow.

class NEFilterControlVerdict

The result from a filter control provider.

class NEFilterVerdict

The abstract base class for filter verdict classes.

class NEFilterReport

The report of the data provider’s action on a flow.

