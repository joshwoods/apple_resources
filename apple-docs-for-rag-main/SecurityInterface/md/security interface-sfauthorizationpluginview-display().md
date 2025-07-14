

- Security Interface
- SFAuthorizationPluginView
-  display() 

Instance Method

# display()

Displays the user interface provided by the authorization plug-in view subclass.

macOS 10.5+

``` source
func display()
```

## Discussion

It’s not likely that you will want to override this method, but if you do, be sure to call `[super displayView]`. If you don’t call `[super displayView]`, your custom view will not get displayed.

This method will raise an SFDisplayViewException exception if an error occurs while displaying the authorization dialog.

## See Also

### Communicating with the Authorization Plug-in

func setButton(SFButtonType, enabled: Bool)

Enables or disables a button in the authorization plug-in’s user interface.

func update()

Tells the authorization plug-in to get and display the appropriate view in the authorization plug-in’s user interface.

