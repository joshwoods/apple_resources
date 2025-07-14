

- Security Interface
- SFAuthorizationView
-  isEnabled() 

Instance Method

# isEnabled()

Indicates whether the authorization view is enabled (true) or disabled (false).

macOS 10.3+

``` source
@MainActor
func isEnabled() -> Bool
```

## Topics

### Related Documentation

func setEnabled(Bool)

Sets the current state of the authorization view.

## See Also

### Getting information about the authorization view

func authorization() -> SFAuthorization!

Returns the authorization object associated with this view.

func authorizationRights() -> UnsafeMutablePointer&lt;AuthorizationRights>!

Returns the authorization rights for this view.

func authorizationState() -> SFAuthorizationViewState

Returns the current state of the authorization view.

