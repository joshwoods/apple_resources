

- Security Interface
- SFAuthorizationPluginView
-  buttonPressed(\_:) 

Instance Method

# buttonPressed(\_:)

Tells the authorization plug-in that the user pressed a button in the custom view.

macOS 10.5+

``` source
func buttonPressed(_ inButtonType: SFButtonType)
```

## Parameters 

`inButtonType`  

The type of button that was pressed.

## Discussion

By default, buttonPressed(_:) will set a result of Deny when the OK or Login buttons are pressed. An SFAuthorizationPluginView subclass needs to override this method to set the context values for the short name of the user so that user attributes can be looked up. To do this, use kAuthorizationEnvironmentUsername as the key. A subclass should also set any additional context values that are needed by the authorization plug-in to verify the user’s credentials. To do this, use the appropriate function pointers you receive from callbacks().

When you override this method, do not call `[super buttonPressed]`.

## See Also

### Responding to User Actions

func view(for: SFViewType) -> NSView!

Returns the appropriate view object for the specified view type.

