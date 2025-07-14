

- HomeKit
- HMEventTrigger
-  updatePredicate(\_:completionHandler:) 

Instance Method

# updatePredicate(\_:completionHandler:)

Replaces the predicate used to evaluate execution of the scene associated with the event trigger.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+

``` source
func updatePredicate(
    _ predicate: NSPredicate?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updatePredicate(_ predicate: NSPredicate?) async throws
```

## Parameters 

`predicate`  

The new predicate to use with the event trigger.

`completion`  

A block that executes after processing the request.

The block takes the following parameter:

error  
If the request was successful, the value of `error` is `nil`; otherwise, the value provides more information about the request status.

## See Also

### Adding a trigger condition

var predicate: NSPredicate?

The predicate to evaluate before executing the scene associated with the event trigger.

