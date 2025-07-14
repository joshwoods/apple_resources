

- Security Interface
- SFAuthorizationPluginView
-  didDeactivate() 

Instance Method

# didDeactivate()

Tells the authorization plug-in that its user interface has been deactivated.

macOS 10.5+

``` source
func didDeactivate()
```

## See Also

### Configuring the User Interface

func didActivate()

Tells the authorization plug-in when its user interface has become active.

func willActivate(withUser: [AnyHashable : Any]!)

Tells the authorization plug-in that its user interface is about to be made active by the Apple-provided Security Agent.

