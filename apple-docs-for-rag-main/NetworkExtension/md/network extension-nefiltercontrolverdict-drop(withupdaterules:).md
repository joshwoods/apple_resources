

- Network Extension
- NEFilterControlVerdict
-  drop(withUpdateRules:) 

Type Method

# drop(withUpdateRules:)

Create a verdict that indicates to the system that all of the flow’s data should be dropped, and that the filtering rules have been updated.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func drop(withUpdateRules updateRules: Bool) -> NEFilterControlVerdict
```

## Parameters 

`updateRules`  

A Boolean indicating whether or not the Filter Control Provider updated the rules.

## Return Value

An `NEFilterControlVerdict` object.

## Discussion

When the Filter Control Provider passes this verdict to the completion handler passed to its handleNewFlow(_:completionHandler:) method, the system will drop all of the flow’s data. In addition, if the updateRules parameter is YES the system will call the Filter Data Provider’s handleRulesChanged() method.

## See Also

### Creating control verdicts

class func allow(withUpdateRules: Bool) -> NEFilterControlVerdict

Create a verdict that indicates to the system that all of the flow’s data should be allowed to pass to its final destination, and that the filtering rules have been updated.

class func updateRules() -> NEFilterControlVerdict

Create a verdict that indicates to the system that the filtering rules have been updated, and that the Filter Data Provider needs to make a decision about the flow’s data.

