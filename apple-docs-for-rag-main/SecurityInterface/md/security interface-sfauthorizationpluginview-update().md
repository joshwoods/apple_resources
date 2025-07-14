

- Security Interface
- SFAuthorizationPluginView
-  update() 

Instance Method

# update()

Tells the authorization plug-in to get and display the appropriate view in the authorization plug-in’s user interface.

macOS 10.5+

``` source
func update()
```

## Discussion

Your subclass of SFAuthorizationPluginView should call this method when a user clicks a button in your view that should result in a new view being displayed. Calling this method causes the authorization plug-in to get the new view and display it.

## See Also

### Communicating with the Authorization Plug-in

func display()

Displays the user interface provided by the authorization plug-in view subclass.

func setButton(SFButtonType, enabled: Bool)

Enables or disables a button in the authorization plug-in’s user interface.

