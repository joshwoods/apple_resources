

- Security Interface
- SFAuthorizationPluginView
-  didActivate() 

Instance Method

# didActivate()

Tells the authorization plug-in when its user interface has become active.

macOS 10.5+

``` source
func didActivate()
```

## See Also

### Configuring the User Interface

func didDeactivate()

Tells the authorization plug-in that its user interface has been deactivated.

func willActivate(withUser: [AnyHashable : Any]!)

Tells the authorization plug-in that its user interface is about to be made active by the Apple-provided Security Agent.

