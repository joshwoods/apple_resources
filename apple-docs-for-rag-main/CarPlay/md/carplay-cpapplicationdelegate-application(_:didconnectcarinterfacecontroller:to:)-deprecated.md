

- CarPlay
- CPApplicationDelegate
-  application(\_:didConnectCarInterfaceController:to:) Deprecated

Instance Method

# application(\_:didConnectCarInterfaceController:to:)

Tells the app delegate that the app connected to the CarPlay interface.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func application(
    _ application: UIApplication,
    didConnectCarInterfaceController interfaceController: CPInterfaceController,
    to window: CPWindow
)
```

**Required**

## Parameters 

`application`  

Your singleton app object.

`interfaceController`  

The interface controller provided by CarPlay. Your app should maintain a reference to this controller.

`window`  

The CarPlay window. Your app should create its view controller and assign the controller to the rootViewController property of this window.

## See Also

### Connecting to the CarPlay Interface

func application(UIApplication, didDisconnectCarInterfaceController: CPInterfaceController, from: CPWindow)

Tells the app delegate that the app disconnected from the CarPlay interface.

**Required**

Deprecated

