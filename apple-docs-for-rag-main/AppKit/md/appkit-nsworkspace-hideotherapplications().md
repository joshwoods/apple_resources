

- AppKit
- NSWorkspace
-  hideOtherApplications() 

Instance Method

# hideOtherApplications()

Hides all applications other than the sender.

macOS

``` source
func hideOtherApplications()
```

## Discussion

In order to hide all apps except the current one, the user can Command-Option-click an app’s Dock icon.

You must call this method from your app’s main thread.

## See Also

### Launching and Hiding Apps

func openApplication(at: URL, configuration: NSWorkspace.OpenConfiguration, completionHandler: ((NSRunningApplication?, (any Error)?) -> Void)?)

Launches the app at the specified URL and asynchronously reports back on the app’s status.

