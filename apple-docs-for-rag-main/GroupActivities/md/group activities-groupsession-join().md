

- Group Activities
- GroupSession
-  join() 

Instance Method

# join()

Starts the shared activity on the current device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final func join()
```

## Mentioned in 

Joining and managing a shared activity

Adding spatial Persona support to an activity

## Discussion

Call this method to begin the delivery of synchronized data to the current device. Typically, you call this method when your app is ready to engage in an activity. For example, call it when you present your app’s UI for the activity. When your app successfully joins the session, the session changes the value in its state property to GroupSession.State.joined.

## See Also

### Joining and leaving the session

func leave()

Leaves the current activity and stops receiving synchronized data.

func end()

Ends the activity for the entire group and stops the transfer of synchronized data.

