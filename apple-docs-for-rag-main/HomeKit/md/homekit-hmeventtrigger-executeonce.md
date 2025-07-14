

- HomeKit
- HMEventTrigger
-  executeOnce 

Instance Property

# executeOnce

A Boolean that can execute the trigger many times.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var executeOnce: Bool { get }
```

## Discussion

Disables the trigger after its first execution if true.

## See Also

### Controlling recurrence

var recurrences: [DateComponents]?

Specifies the days on which the trigger can execute.

func updateRecurrences([DateComponents]?, completionHandler: ((any Error)?) -> Void)

Updates the days of the week the trigger can repeat.

func updateExecuteOnce(Bool, completionHandler: ((any Error)?) -> Void)

Updates the repetition status of the event trigger.

