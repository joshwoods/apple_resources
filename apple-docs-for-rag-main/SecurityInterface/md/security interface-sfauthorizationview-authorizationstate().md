

- Security Interface
- SFAuthorizationView
-  authorizationState() 

Instance Method

# authorizationState()

Returns the current state of the authorization view.

macOS 10.3+

``` source
@MainActor
func authorizationState() -> SFAuthorizationViewState
```

## Topics

### Related Documentation

func deauthorize(Any!) -> Bool

Sets the authorization state to unauthorized and locks the lock icon in the view.

func authorize(Any!) -> Bool

Attempts to unlock the lock icon in the view.

## See Also

### Getting information about the authorization view

func authorization() -> SFAuthorization!

Returns the authorization object associated with this view.

func authorizationRights() -> UnsafeMutablePointer&lt;AuthorizationRights>!

Returns the authorization rights for this view.

func isEnabled() -> Bool

Indicates whether the authorization view is enabled (true) or disabled (false).

