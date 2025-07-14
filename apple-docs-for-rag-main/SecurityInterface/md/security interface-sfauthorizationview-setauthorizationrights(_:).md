

- Security Interface
- SFAuthorizationView
-  setAuthorizationRights(\_:) 

Instance Method

# setAuthorizationRights(\_:)

Sets the authorization rights for this view.

macOS 10.3+

``` source
@MainActor
func setAuthorizationRights(_ authorizationRights: UnsafePointer!)
```

## Parameters 

`authorizationRights`  

An authorization rights structure specifying the authorization rights represented by the authorization view.

## Discussion

Either this method or the setString(_:) method must be called before the view displays correctly.

The authorization rights structures are defined in AuthorizationRights in Authorization Services.

## See Also

### Related Documentation

func authorizationRights() -> UnsafeMutablePointer&lt;AuthorizationRights>!

Returns the authorization rights for this view.

### Setting up the authorization view

func setString(AuthorizationString!)

Sets the requested-right string to use with the default authorization rights set.

func setAutoupdate(Bool)

Sets the authorization view to update itself automatically.

func setAutoupdate(Bool, interval: TimeInterval)

Sets the authorization view to update itself at a specific interval.

func setFlags(AuthorizationFlags)

Sets the current authorization flags for the view.

func setEnabled(Bool)

Sets the current state of the authorization view.

