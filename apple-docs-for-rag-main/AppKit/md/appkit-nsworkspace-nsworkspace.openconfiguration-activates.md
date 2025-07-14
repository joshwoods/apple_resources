

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  activates 

Instance Property

# activates

A Boolean value indicating whether the system activates the app and brings it to the foreground.

macOS 10.15+

``` source
var activates: Bool { get set }
```

## Discussion

The default value of this property is true, which causes the system to bring the app to the foreground.

## See Also

### Specifying App-Related Behaviors

var addsToRecentItems: Bool

A Boolean value indicating whether to add the app or documents to the Recent Items menu.

var allowsRunningApplicationSubstitution: Bool

A Boolean value that indicates whether to use a running instance of an application even if it’s at a different URL.

var createsNewApplicationInstance: Bool

A Boolean value indicating whether you want the system to launch a new instance of the app.

var hides: Bool

A Boolean value indicating whether you want the app to hide itself after it launches.

var hidesOthers: Bool

A Boolean value indicating whether you want to hide all apps except the one that launched.

