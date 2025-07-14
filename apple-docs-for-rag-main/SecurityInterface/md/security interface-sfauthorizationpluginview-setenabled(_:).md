

- Security Interface
- SFAuthorizationPluginView
-  setEnabled(\_:) 

Instance Method

# setEnabled(\_:)

Enables or disables the controls in the authorization plug-in’s view.

macOS 10.5+

``` source
func setEnabled(_ inEnabled: Bool)
```

## Parameters 

`inEnabled`  

The state the controls should be in.

## Discussion

When the authorization plug-in calls this method, the subclass should call setEnabled(_:) on the controls that are in its view.

