

- Security Interface
- SFAuthorizationView
-  updateStatus(\_:) 

Instance Method

# updateStatus(\_:)

Manually updates the authorization view.

macOS 10.3+

``` source
@MainActor
func updateStatus(_ inSender: Any!) -> Bool
```

## Parameters 

`inSender`  

The authorization view to update.

## Discussion

Calls to updateStatus(_:) return true if in the unlocked state, false otherwise.

If autoupdates have not been set, you must call updateStatus(_:) for the authorization view’s initial state to display correctly. The Security Framework calls this method for you when you change the state of the lock (by calling deauthorize(_:), for example).

## See Also

### Related Documentation

func setAutoupdate(Bool)

Sets the authorization view to update itself automatically.

func setAutoupdate(Bool, interval: TimeInterval)

Sets the authorization view to update itself at a specific interval.

