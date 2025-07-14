

- Security Interface
- SFAuthorizationPluginView
-  view(for:) 

Instance Method

# view(for:)

Returns the appropriate view object for the specified view type.

macOS 10.5+

``` source
func view(for inType: SFViewType) -> NSView!
```

## Parameters 

`inType`  

The type of view being requested by the authorization plug-in.

## Return Value

An NSView object representing either a credentials view or an identity and credentials view.

## Discussion

When the authorization plug-in calls this method, the SFAuthorizationPluginView instance should return the NSView object that represents the view indicated by the specified SFViewType. The NSView object and its contents should have the autoresize flags set to allow the view to be resized.

Note that although a maximum width of 394 points is currently supported, this may change in the future. You should not assume that the width of the NSView object will never change.

## See Also

### Responding to User Actions

func buttonPressed(SFButtonType)

Tells the authorization plug-in that the user pressed a button in the custom view.

