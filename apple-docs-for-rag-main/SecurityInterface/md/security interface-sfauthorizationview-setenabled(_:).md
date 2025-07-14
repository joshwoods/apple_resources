

- Security Interface
- SFAuthorizationView
-  setEnabled(\_:) 

Instance Method

# setEnabled(\_:)

Sets the current state of the authorization view.

macOS 10.3+

``` source
@MainActor
func setEnabled(_ enabled: Bool)
```

## Parameters 

`enabled`  

Specifies whether the authorization view should be enabled (true) or disabled (false).

## Discussion

A disabled view is visible but dimmed.

## Topics

### Related Documentation

func authorizationState() -> SFAuthorizationViewState

Returns the current state of the authorization view.

## See Also

### Setting up the authorization view

func setString(AuthorizationString!)

Sets the requested-right string to use with the default authorization rights set.

func setAuthorizationRights(UnsafePointer&lt;AuthorizationRights>!)

Sets the authorization rights for this view.

func setAutoupdate(Bool)

Sets the authorization view to update itself automatically.

func setAutoupdate(Bool, interval: TimeInterval)

Sets the authorization view to update itself at a specific interval.

func setFlags(AuthorizationFlags)

Sets the current authorization flags for the view.

