

- HomeKit
- HMEventTrigger
-  updateRecurrences(\_:completionHandler:) 

Instance Method

# updateRecurrences(\_:completionHandler:)

Updates the days of the week the trigger can repeat.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func updateRecurrences(
    _ recurrences: [DateComponents]?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateRecurrences(_ recurrences: [DateComponents]?) async throws
```

## Parameters 

`recurrences`  

An array of DateComponents that represent the days of the week that the event trigger can repeat. Only respects the weekday property of DateComponents.

`completion`  

A block that executes after processing the request.

The block takes the following parameter:

error  
If the request was successful, the value of `error` is `nil`; otherwise, the value provides more information about the request status.

## See Also

### Controlling recurrence

var recurrences: [DateComponents]?

Specifies the days on which the trigger can execute.

var executeOnce: Bool

A Boolean that can execute the trigger many times.

func updateExecuteOnce(Bool, completionHandler: ((any Error)?) -> Void)

Updates the repetition status of the event trigger.

