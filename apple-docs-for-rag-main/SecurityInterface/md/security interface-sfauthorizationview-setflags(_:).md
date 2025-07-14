

- Security Interface
- SFAuthorizationView
-  setFlags(\_:) 

Instance Method

# setFlags(\_:)

Sets the current authorization flags for the view.

macOS 10.3+

``` source
@MainActor
func setFlags(_ flags: AuthorizationFlags)
```

## Parameters 

`flags`  

The authorization flags to set for this view.

## Discussion

You can use this method to change the authorization flag settings made with the setAuthorizationRights(_:) method or to specify flags other than the default (kAuthorizationFlagDefaults) used by the setString(_:) method.

The authorization flags are described in Authorization Options in Authorization Services.

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

func setEnabled(Bool)

Sets the current state of the authorization view.

