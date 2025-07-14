

- AppKit
- NSApplication
-  disableRelaunchOnLogin() 

Instance Method

# disableRelaunchOnLogin()

Disables relaunching the app on login.

macOS 10.7+

``` source
@MainActor
func disableRelaunchOnLogin()
```

## Discussion

Invoking this method will prevent the app from relaunching when the user next logs in to their account.

If your app shouldn’t be relaunched because it launches via some other mechanism (for example, `launchd`), then the recommended usage is to call this method once, and never pair it with an enableRelaunchOnLogin() method.

If your app shouldn’t be relaunched because it triggers a restart, for example an installer, then the recommended usage is to invoke this method immediately before you attempt to trigger a restart, and enableRelaunchOnLogin() immediately after. This is because the user may cancel restarting; if the user later restarts for another reason, then your app should be brought back.

This methods is thread safe.

## See Also

### Managing Relaunch on Login

func enableRelaunchOnLogin()

Enables relaunching the app on login.

