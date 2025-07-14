

- Core Spotlight
- CSSearchableItemAttributeSet
-  supportsNavigation 

Instance Property

# supportsNavigation

A value that indicates whether the item contains information sufficient to provide navigation to the location it represents.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var supportsNavigation: NSNumber? { get set }
```

## Mentioned in 

Adding your app’s content to Spotlight indexes

## Discussion

When an item includes latitude and longitude properties, these properties can be used for navigation to the location represented by the item. For example, it makes sense to set supportsNavigation to `1` for an item that represents review for a specific restaurant, but not for an item that represents a photo of a person.

## See Also

### Supporting actions

var actionIdentifiers: [String]

The identifiers that specify custom actions the app supports for the item.

var supportsPhoneCall: NSNumber?

A value that indicates whether the item contains information sufficient to allow a phone call to a number associated with the item.

var sharedItemContentType: UTType?

The file type of the item to enable the user to share items from Spotlight.

let CSActionIdentifier: String

A key that specifies the action’s identifier in a user activity.

