

- HomeKit
- HMTimerTrigger
-  updateFireDate(\_:completionHandler:) 

Instance Method

# updateFireDate(\_:completionHandler:)

Updates the next fire date for the trigger.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func updateFireDate(
    _ fireDate: Date,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateFireDate(_ fireDate: Date) async throws
```

## Parameters 

`fireDate`  

The new fire date.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Choosing the fire date

var fireDate: Date

The time at which the trigger will next fire.

