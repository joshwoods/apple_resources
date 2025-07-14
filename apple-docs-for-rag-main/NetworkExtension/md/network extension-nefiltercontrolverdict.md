

- Network Extension
-  NEFilterControlVerdict 

Class

# NEFilterControlVerdict

The result from a filter control provider.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEFilterControlVerdict
```

## Topics

### Creating control verdicts

class func allow(withUpdateRules: Bool) -> NEFilterControlVerdict

Create a verdict that indicates to the system that all of the flow’s data should be allowed to pass to its final destination, and that the filtering rules have been updated.

class func drop(withUpdateRules: Bool) -> NEFilterControlVerdict

Create a verdict that indicates to the system that all of the flow’s data should be dropped, and that the filtering rules have been updated.

class func updateRules() -> NEFilterControlVerdict

Create a verdict that indicates to the system that the filtering rules have been updated, and that the Filter Data Provider needs to make a decision about the flow’s data.

## Relationships

### Inherits From

- NEFilterNewFlowVerdict

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

class NEFilterRemediationVerdict

The result from a filter data provider after the user requests remediation for a blocked flow.

class NEFilterVerdict

The abstract base class for filter verdict classes.

class NEFilterReport

The report of the data provider’s action on a flow.

