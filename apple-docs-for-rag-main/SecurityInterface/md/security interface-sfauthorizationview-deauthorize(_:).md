

- Security Interface
- SFAuthorizationView
-  deauthorize(\_:) 

Instance Method

# deauthorize(\_:)

Sets the authorization state to unauthorized and locks the lock icon in the view.

macOS 10.3+

``` source
@MainActor
func deauthorize(_ inSender: Any!) -> Bool
```

## Parameters 

`inSender`  

The authorization view to lock.

## Discussion

If this method succeeds, it returns true; if it fails, the lock icon remains unlocked and the method returns false.

## See Also

### Setting the authorization state

func authorize(Any!) -> Bool

Attempts to unlock the lock icon in the view.

