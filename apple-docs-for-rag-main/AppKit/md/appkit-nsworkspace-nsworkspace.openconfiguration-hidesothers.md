

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  hidesOthers 

Instance Property

# hidesOthers

A Boolean value indicating whether you want to hide all apps except the one that launched.

macOS 10.15+

``` source
var hidesOthers: Bool { get set }
```

## Discussion

The default value of this property is false, which leaves the visibility of other apps unchanged. Setting the property to true hides all apps except the one that launched.

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

var hides: Bool

A Boolean value indicating whether you want the app to hide itself after it launches.

