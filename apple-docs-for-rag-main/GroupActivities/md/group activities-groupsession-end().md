

- Group Activities
- GroupSession
-  end() 

Instance Method

# end()

Ends the activity for the entire group and stops the transfer of synchronized data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final func end()
```

## Mentioned in 

Joining and managing a shared activity

## Discussion

Call this method to end the activity for all participants. When you call this method, the session transitions to the GroupSession.State.invalidated(reason:) state and stops the delivery of session-related updates. After ending the session, you can’t join it again.

Don’t call this method on a session already in the GroupSession.State.invalidated(reason:) state.

## See Also

### Joining and leaving the session

func join()

Starts the shared activity on the current device.

func leave()

Leaves the current activity and stops receiving synchronized data.

