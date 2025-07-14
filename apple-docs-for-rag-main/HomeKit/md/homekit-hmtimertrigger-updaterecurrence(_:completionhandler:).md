

- HomeKit
- HMTimerTrigger
-  updateRecurrence(\_:completionHandler:) 

Instance Method

# updateRecurrence(\_:completionHandler:)

Updates the recurrence interval.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func updateRecurrence(
    _ recurrence: DateComponents?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateRecurrence(_ recurrence: DateComponents?) async throws
```

## Parameters 

`recurrence`  

The new recurrence interval.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

See recurrence for a discussion of how the recurrence value is used.

## See Also

### Using recurrence

var recurrence: DateComponents?

The interval on which to repeat firing the trigger.

