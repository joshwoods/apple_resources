

- Security Interface
- SFAuthorizationView
-  setString(\_:) 

Instance Method

# setString(\_:)

Sets the requested-right string to use with the default authorization rights set.

macOS 10.3+

``` source
@MainActor
func setString(_ authorizationString: AuthorizationString!)
```

## Parameters 

`authorizationString`  

The string to be displayed.

## Discussion

This is a convenience method that creates an authorization rights set when you specify only the name of the requested right. The requested-right string is displayed in the Details pane of the user authentication dialog box. Either this method or the setAuthorizationRights(_:) method must be called before the view displays correctly.

## See Also

### Related Documentation

Authorization Services Programming Guide

func authorizationRights() -> UnsafeMutablePointer&lt;AuthorizationRights>!

Returns the authorization rights for this view.

### Setting up the authorization view

func setAuthorizationRights(UnsafePointer&lt;AuthorizationRights>!)

Sets the authorization rights for this view.

func setAutoupdate(Bool)

Sets the authorization view to update itself automatically.

func setAutoupdate(Bool, interval: TimeInterval)

Sets the authorization view to update itself at a specific interval.

func setFlags(AuthorizationFlags)

Sets the current authorization flags for the view.

func setEnabled(Bool)

Sets the current state of the authorization view.

