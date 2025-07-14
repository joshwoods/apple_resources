

- Core Spotlight
-  CSActionIdentifier 

Global Variable

# CSActionIdentifier

A key that specifies the action’s identifier in a user activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
let CSActionIdentifier: String
```

## Discussion

When the user selects a custom action on an indexed item, the system launches your app and invokes application(_:continue:restorationHandler:). The `userInfo` dictionary of the specified NSUserActivity includes the corresponding `Info.plist` using this key.

## See Also

### Supporting actions

var actionIdentifiers: [String]

The identifiers that specify custom actions the app supports for the item.

var supportsNavigation: NSNumber?

A value that indicates whether the item contains information sufficient to provide navigation to the location it represents.

var supportsPhoneCall: NSNumber?

A value that indicates whether the item contains information sufficient to allow a phone call to a number associated with the item.

var sharedItemContentType: UTType?

The file type of the item to enable the user to share items from Spotlight.

