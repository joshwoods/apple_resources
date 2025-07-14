

- TVMLKit JS
- App
-  onSuspend 

Instance Property

# onSuspend

A callback function that is automatically called when the app is sent to the background.

tvOS 9.0+

``` source
attribute function onSuspend;
```

## Discussion

Use the `onSuspend` attribute to stop any actions when the app moves from the foreground to the background. This attribute must be set to a function that accepts an `options` argument; for example `App.onSuspend = function (options) {}`. The `options` argument is always set to `null`.

## See Also

### Responding to App Life Cycle Events

onError

A callback function that is automatically called when an error is sent from the Apple TV.

onExit

A callback function that is automatically called when the app has been exited.

onLaunch

A callback function that is automatically called when the app has been launched.

onResume

A callback function that is automatically called when the app moves to the foreground.

