

- Network Extension
- NEFilterControlVerdict
-  updateRules() 

Type Method

# updateRules()

Create a verdict that indicates to the system that the filtering rules have been updated, and that the Filter Data Provider needs to make a decision about the flow’s data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func updateRules() -> NEFilterControlVerdict
```

## Return Value

An `NEFilterControlVerdict` object.

## See Also

### Creating control verdicts

class func allow(withUpdateRules: Bool) -> NEFilterControlVerdict

Create a verdict that indicates to the system that all of the flow’s data should be allowed to pass to its final destination, and that the filtering rules have been updated.

class func drop(withUpdateRules: Bool) -> NEFilterControlVerdict

Create a verdict that indicates to the system that all of the flow’s data should be dropped, and that the filtering rules have been updated.

