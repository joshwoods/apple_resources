

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  createsNewApplicationInstance 

Instance Property

# createsNewApplicationInstance

A Boolean value indicating whether you want the system to launch a new instance of the app.

macOS 10.15+

``` source
var createsNewApplicationInstance: Bool { get set }
```

## Discussion

When the value of this property is true, the system always launches a new version of the app, even if an existing copy is already running. The default value of this property is false, which causes the system to open the already running app when present.

## See Also

### Specifying App-Related Behaviors

var activates: Bool

A Boolean value indicating whether the system activates the app and brings it to the foreground.

var addsToRecentItems: Bool

A Boolean value indicating whether to add the app or documents to the Recent Items menu.

var allowsRunningApplicationSubstitution: Bool

A Boolean value that indicates whether to use a running instance of an application even if it’s at a different URL.

var hides: Bool

A Boolean value indicating whether you want the app to hide itself after it launches.

var hidesOthers: Bool

A Boolean value indicating whether you want to hide all apps except the one that launched.

