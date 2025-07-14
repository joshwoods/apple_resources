

- TVMLKit JS
- App
-  onExit 

Instance Property

# onExit

A callback function that is automatically called when the app has been exited.

tvOS 9.0+

``` source
attribute function onExit;
```

## Discussion

Use the `onExit` attribute to complete any actions that need to be cleaned up (for example, releasing any system resources) when the app has been exited. This attribute must be set to a function that accepts an `options` argument; for example `App.onExit = function (options) {}`. The options argument can contain the following keys:

- `reloading`—Set to `true` if the app is exiting as a result of `App.reload()` and is to be relaunched later.

## See Also

### Responding to App Life Cycle Events

onError

A callback function that is automatically called when an error is sent from the Apple TV.

onLaunch

A callback function that is automatically called when the app has been launched.

onResume

A callback function that is automatically called when the app moves to the foreground.

onSuspend

A callback function that is automatically called when the app is sent to the background.

