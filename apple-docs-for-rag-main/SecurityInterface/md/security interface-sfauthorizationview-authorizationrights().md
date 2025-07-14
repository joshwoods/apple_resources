

- Security Interface
- SFAuthorizationView
-  authorizationRights() 

Instance Method

# authorizationRights()

Returns the authorization rights for this view.

macOS 10.3+

``` source
@MainActor
func authorizationRights() -> UnsafeMutablePointer!
```

## See Also

### Related Documentation

func setAuthorizationRights(UnsafePointer&lt;AuthorizationRights>!)

Sets the authorization rights for this view.

### Getting information about the authorization view

func authorization() -> SFAuthorization!

Returns the authorization object associated with this view.

func authorizationState() -> SFAuthorizationViewState

Returns the current state of the authorization view.

func isEnabled() -> Bool

Indicates whether the authorization view is enabled (true) or disabled (false).

