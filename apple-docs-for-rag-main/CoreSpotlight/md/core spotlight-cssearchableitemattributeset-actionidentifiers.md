

- Core Spotlight
- CSSearchableItemAttributeSet
-  actionIdentifiers 

Instance Property

# actionIdentifiers

The identifiers that specify custom actions the app supports for the item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var actionIdentifiers: [String] { get set }
```

## Discussion

The identifiers correspond to the CoreSpotlightActionIdentifier values you specify in the CoreSpotlightActions key of the app’s `Info.plist` file.

When the user selects a custom action on an indexed item, the system launches your app and invokes application(_:continue:restorationHandler:). The `userInfo` dictionary of the specified NSUserActivity includes the corresponding `Info.plist` entry using the key CSActionIdentifier.

## See Also

### Supporting actions

var supportsNavigation: NSNumber?

A value that indicates whether the item contains information sufficient to provide navigation to the location it represents.

var supportsPhoneCall: NSNumber?

A value that indicates whether the item contains information sufficient to allow a phone call to a number associated with the item.

var sharedItemContentType: UTType?

The file type of the item to enable the user to share items from Spotlight.

let CSActionIdentifier: String

A key that specifies the action’s identifier in a user activity.

