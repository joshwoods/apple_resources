

- TVMLKit JS
- App
-  onError 

Instance Property

# onError

A callback function that is automatically called when an error is sent from the Apple TV.

tvOS 9.0+

``` source
attribute function onError;
```

## Discussion

Use the `onError` attribute to handle any errors sent from the Apple TV. This attribute must be set to the following function: `App.onError = function (message, sourceURL, line) {}`.

- `message`—The error message.

- `sourceURL`—The URL for the TVMLKit JS file where the error occurred. Defaults to `nil` if the information is not available.

- `line`—The line in the TVMLKit JS file where the error occurred. Defaults to `nil` if the information is not available.

## See Also

### Responding to App Life Cycle Events

onExit

A callback function that is automatically called when the app has been exited.

onLaunch

A callback function that is automatically called when the app has been launched.

onResume

A callback function that is automatically called when the app moves to the foreground.

onSuspend

A callback function that is automatically called when the app is sent to the background.

