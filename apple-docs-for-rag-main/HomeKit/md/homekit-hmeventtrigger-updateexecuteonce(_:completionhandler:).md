

- HomeKit
- HMEventTrigger
-  updateExecuteOnce(\_:completionHandler:) 

Instance Method

# updateExecuteOnce(\_:completionHandler:)

Updates the repetition status of the event trigger.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func updateExecuteOnce(
    _ executeOnce: Bool,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateExecuteOnce(_ executeOnce: Bool) async throws
```

## Parameters 

`executeOnce`  

A Boolean value that specifies whether to repeat the trigger.

`completion`  

A block that executes after processing the request.

The block takes the following parameter:

error  
If the request was successful, the value of `error` is `nil`; otherwise, the value provides more information about the request status.

## See Also

### Controlling recurrence

var recurrences: [DateComponents]?

Specifies the days on which the trigger can execute.

func updateRecurrences([DateComponents]?, completionHandler: ((any Error)?) -> Void)

Updates the days of the week the trigger can repeat.

var executeOnce: Bool

A Boolean that can execute the trigger many times.

