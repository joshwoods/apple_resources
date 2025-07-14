

- TVMLKit JS
- App
-  onLaunch 

Instance Property

# onLaunch

A callback function that is automatically called when the app has been launched.

tvOS 9.0+

``` source
attribute function onLaunch;
```

## Discussion

Use the `onLaunch` attribute to start any required actions (for example, loading the first TVML page) when the app launches. This attribute must be set to a function that accepts an `options` argument; for example `App.onLaunch = function (options) {}`. The options argument can contain the following keys:

- `launchContext`—Determines how the app is launched. Set to `background` to launch the app in the background.

- `location`—Contains the boot TVMLKit JS URL location.

- `reloadData`—The object passed in to `App.reload()` when the app is relaunched.

- User defined keys—Any custom keys that were passed to launchOptions.

## See Also

### Responding to App Life Cycle Events

onError

A callback function that is automatically called when an error is sent from the Apple TV.

onExit

A callback function that is automatically called when the app has been exited.

onResume

A callback function that is automatically called when the app moves to the foreground.

onSuspend

A callback function that is automatically called when the app is sent to the background.

