

- Security Interface
- SFAuthorizationView
-  setAutoupdate(\_:interval:) 

Instance Method

# setAutoupdate(\_:interval:)

Sets the authorization view to update itself at a specific interval.

macOS 10.3+

``` source
@MainActor
func setAutoupdate(
    _ autoupdate: Bool,
    interval: TimeInterval
)
```

## Parameters 

`autoupdate`  

Specifies whether the authorization view should update itself automatically. Set to true to enable autoupdates.

`interval`  

If `autoupdate` is true, sets the interval at which updates take place, in seconds.

## Discussion

If autoupdates are enabled and the authorization times out (for example), the authorization view automatically relocks. If autoupdates are disabled, you have to call the updateStatus(_:) method to manually update the view if the status changes when the user has not clicked on the lock icon. Autoupdates are disabled by default. Because autoupdates poll, they can affect system performance. For that reason, you might want to set a time interval so that the polling does not take place as often.

## See Also

### Setting up the authorization view

func setString(AuthorizationString!)

Sets the requested-right string to use with the default authorization rights set.

func setAuthorizationRights(UnsafePointer&lt;AuthorizationRights>!)

Sets the authorization rights for this view.

func setAutoupdate(Bool)

Sets the authorization view to update itself automatically.

func setFlags(AuthorizationFlags)

Sets the current authorization flags for the view.

func setEnabled(Bool)

Sets the current state of the authorization view.

