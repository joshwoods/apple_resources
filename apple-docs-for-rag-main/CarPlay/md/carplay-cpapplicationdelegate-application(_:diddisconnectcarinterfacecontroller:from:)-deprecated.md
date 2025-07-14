

- CarPlay
- CPApplicationDelegate
-  application(\_:didDisconnectCarInterfaceController:from:) Deprecated

Instance Method

# application(\_:didDisconnectCarInterfaceController:from:)

Tells the app delegate that the app disconnected from the CarPlay interface.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func application(
    _ application: UIApplication,
    didDisconnectCarInterfaceController interfaceController: CPInterfaceController,
    from window: CPWindow
)
```

**Required**

## Parameters 

`application`  

Your singleton app object.

`interfaceController`  

The interface controller provided by CarPlay. Your app should release its reference to this controller.

`window`  

The CarPlay window.

## See Also

### Connecting to the CarPlay Interface

func application(UIApplication, didConnectCarInterfaceController: CPInterfaceController, to: CPWindow)

Tells the app delegate that the app connected to the CarPlay interface.

**Required**

Deprecated

