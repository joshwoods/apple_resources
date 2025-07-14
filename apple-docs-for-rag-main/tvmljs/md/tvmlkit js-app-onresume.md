

- TVMLKit JS
- App
-  onResume 

Instance Property

# onResume

A callback function that is automatically called when the app moves to the foreground.

tvOS 9.0+

``` source
attribute function onResume;
```

## Discussion

Use the `onResume` attribute to start any required actions when the app moves from the background to the foreground. This attribute must be set to a function that accepts an `options` argument; for example `App.onResume = function (options) {}`. The `options` argument is always set to `null`.

## See Also

### Responding to App Life Cycle Events

onError

A callback function that is automatically called when an error is sent from the Apple TV.

onExit

A callback function that is automatically called when the app has been exited.

onLaunch

A callback function that is automatically called when the app has been launched.

onSuspend

A callback function that is automatically called when the app is sent to the background.

