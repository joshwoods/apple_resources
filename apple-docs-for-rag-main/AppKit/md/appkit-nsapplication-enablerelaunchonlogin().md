

- AppKit
- NSApplication
-  enableRelaunchOnLogin() 

Instance Method

# enableRelaunchOnLogin()

Enables relaunching the app on login.

macOS 10.7+

``` source
@MainActor
func enableRelaunchOnLogin()
```

## Discussion

Invoking this method will cause the app to relaunch when the user next logs in to their account.

This methods is thread safe.

## See Also

### Managing Relaunch on Login

func disableRelaunchOnLogin()

Disables relaunching the app on login.

