

- CarPlay
- CPApplicationDelegate
-  application(\_:didSelect:) Deprecated

Instance Method

# application(\_:didSelect:)

Tells the app delegate that the user selected an action from a navigation alert.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
optional func application(
    _ application: UIApplication,
    didSelect navigationAlert: CPNavigationAlert
)
```

## Parameters 

`application`  

Your singleton app object.

`navigationAlert`  

The alert tapped by the user.

## Discussion

When your app posts a navigation alert while running in the background, CarPlay may display a notification banner. If the user taps the banner, the system displays your app on the CarPlay screen, then calls this method.

