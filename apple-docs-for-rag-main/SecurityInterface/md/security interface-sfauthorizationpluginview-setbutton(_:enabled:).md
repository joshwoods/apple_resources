

- Security Interface
- SFAuthorizationPluginView
-  setButton(\_:enabled:) 

Instance Method

# setButton(\_:enabled:)

Enables or disables a button in the authorization plug-in’s user interface.

macOS 10.5+

``` source
func setButton(
    _ inButtonType: SFButtonType,
    enabled inEnabled: Bool
)
```

## Parameters 

`inButtonType`  

The type of the button.

`inEnabled`  

true to enable the button, false to disable the button.

## See Also

### Communicating with the Authorization Plug-in

func display()

Displays the user interface provided by the authorization plug-in view subclass.

func update()

Tells the authorization plug-in to get and display the appropriate view in the authorization plug-in’s user interface.

