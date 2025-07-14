

- Security Interface
- SFAuthorizationView
-  authorize(\_:) 

Instance Method

# authorize(\_:)

Attempts to unlock the lock icon in the view.

macOS 10.3+

``` source
@MainActor
func authorize(_ inSender: Any!) -> Bool
```

## Parameters 

`inSender`  

The authorization view to unlock.

## Discussion

This method has the same behavior as if the user clicked on the lock icon; if the user is authorized, the lock icon unlocks. If this method succeeds, it returns true; if it fails, the lock icon remains locked and the method returns false.

## See Also

### Related Documentation

func deauthorize(Any!) -> Bool

Sets the authorization state to unauthorized and locks the lock icon in the view.

func authorizationState() -> SFAuthorizationViewState

Returns the current state of the authorization view.

### Setting the authorization state

func deauthorize(Any!) -> Bool

Sets the authorization state to unauthorized and locks the lock icon in the view.

