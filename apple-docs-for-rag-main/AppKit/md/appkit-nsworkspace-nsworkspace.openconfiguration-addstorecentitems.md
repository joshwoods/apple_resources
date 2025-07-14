

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  addsToRecentItems 

Instance Property

# addsToRecentItems

A Boolean value indicating whether to add the app or documents to the Recent Items menu.

macOS 10.15+

``` source
var addsToRecentItems: Bool { get set }
```

## Discussion

The default value of this property is true, which causes AppKit to add the items to the Recent Items menu.

## See Also

### Specifying App-Related Behaviors

var activates: Bool

A Boolean value indicating whether the system activates the app and brings it to the foreground.

var allowsRunningApplicationSubstitution: Bool

A Boolean value that indicates whether to use a running instance of an application even if it’s at a different URL.

var createsNewApplicationInstance: Bool

A Boolean value indicating whether you want the system to launch a new instance of the app.

var hides: Bool

A Boolean value indicating whether you want the app to hide itself after it launches.

var hidesOthers: Bool

A Boolean value indicating whether you want to hide all apps except the one that launched.

