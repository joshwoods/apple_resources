

- Security Interface
- SFAuthorizationView
-  authorization() 

Instance Method

# authorization()

Returns the authorization object associated with this view.

macOS 10.3+

``` source
@MainActor
func authorization() -> SFAuthorization!
```

## Discussion

The authorization object is defined in Security Foundation.

## See Also

### Getting information about the authorization view

func authorizationRights() -> UnsafeMutablePointer&lt;AuthorizationRights>!

Returns the authorization rights for this view.

func authorizationState() -> SFAuthorizationViewState

Returns the current state of the authorization view.

func isEnabled() -> Bool

Indicates whether the authorization view is enabled (true) or disabled (false).

