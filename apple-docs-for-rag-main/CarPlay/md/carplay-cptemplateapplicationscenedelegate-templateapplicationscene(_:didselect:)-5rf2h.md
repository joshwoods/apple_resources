

- CarPlay
- CPTemplateApplicationSceneDelegate
-  templateApplicationScene(\_:didSelect:) 

Instance Method

# templateApplicationScene(\_:didSelect:)

Tells the delegate when the user selects a maneuver while the app is in the background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func templateApplicationScene(
    _ templateApplicationScene: CPTemplateApplicationScene,
    didSelect maneuver: CPManeuver
)
```

## Parameters 

`templateApplicationScene`  

The active scene.

`maneuver`  

The selected maneuver.

## Discussion

If your navigation app posts a maneuver while in the background, CarPlay displays a notification banner to the user. If the user taps the banner, CarPlay brings your navigation app to the foreground and calls this method.

## See Also

### Responding to User Actions

func templateApplicationScene(CPTemplateApplicationScene, didSelect: CPNavigationAlert)

Tells the delegate when the user selects a navigation alert while the app is in the background.

