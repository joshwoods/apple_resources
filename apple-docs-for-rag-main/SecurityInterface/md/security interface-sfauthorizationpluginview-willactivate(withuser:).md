

- Security Interface
- SFAuthorizationPluginView
-  willActivate(withUser:) 

Instance Method

# willActivate(withUser:)

Tells the authorization plug-in that its user interface is about to be made active by the Apple-provided Security Agent.

macOS 10.5+

``` source
func willActivate(withUser inUserInformation: [AnyHashable : Any]!)
```

## Parameters 

`inUserInformation`  

A dictionary that contains the following information:

- SFAuthorizationPluginViewUserNameKey

An NSString object containing the selected user’s name

- SFAuthorizationPluginViewUserShortNameKey

An NSString object containing the selected user’s short name

Note: `inUserInformation` may be `nil`.

## Discussion

Your SFAuthorizationPluginView instance can use the user name to pre-populate a text field in the user interface.

## See Also

### Configuring the User Interface

func didActivate()

Tells the authorization plug-in when its user interface has become active.

func didDeactivate()

Tells the authorization plug-in that its user interface has been deactivated.

