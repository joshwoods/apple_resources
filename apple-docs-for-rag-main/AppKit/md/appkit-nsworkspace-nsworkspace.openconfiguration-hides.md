

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  hides 

Instance Property

# hides

A Boolean value indicating whether you want the app to hide itself after it launches.

macOS 10.15+

``` source
var hides: Bool { get set }
```

## Discussion

The default value of this property is false, which leaves the app in its default state after launch. Setting the property to true causes the app to hide itself.

## See Also

### Specifying App-Related Behaviors

var activates: Bool

A Boolean value indicating whether the system activates the app and brings it to the foreground.

var addsToRecentItems: Bool

A Boolean value indicating whether to add the app or documents to the Recent Items menu.

var allowsRunningApplicationSubstitution: Bool

A Boolean value that indicates whether to use a running instance of an application even if it’s at a different URL.

var createsNewApplicationInstance: Bool

A Boolean value indicating whether you want the system to launch a new instance of the app.

var hidesOthers: Bool

A Boolean value indicating whether you want to hide all apps except the one that launched.

