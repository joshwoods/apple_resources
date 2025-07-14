

- HomeKit
- HMEventTrigger
-  recurrences 

Instance Property

# recurrences

Specifies the days on which the trigger can execute.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var recurrences: [DateComponents]? { get }
```

## Discussion

This property represents the days of the week that the trigger recurs; the trigger ignores all properties other than weekday on the DateComponents object.

## See Also

### Controlling recurrence

func updateRecurrences([DateComponents]?, completionHandler: ((any Error)?) -> Void)

Updates the days of the week the trigger can repeat.

var executeOnce: Bool

A Boolean that can execute the trigger many times.

func updateExecuteOnce(Bool, completionHandler: ((any Error)?) -> Void)

Updates the repetition status of the event trigger.

