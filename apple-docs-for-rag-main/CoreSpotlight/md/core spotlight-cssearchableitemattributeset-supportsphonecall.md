

- Core Spotlight
- CSSearchableItemAttributeSet
-  supportsPhoneCall 

Instance Property

# supportsPhoneCall

A value that indicates whether the item contains information sufficient to allow a phone call to a number associated with the item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var supportsPhoneCall: NSNumber? { get set }
```

## Mentioned in 

Adding your app’s content to Spotlight indexes

## Discussion

When an item includes the phoneNumbers property, the phone number can be used to initiate phone calls. You can use the supportsPhoneCall property to indicate when making a phone call is appropriate and likely to be a primary action for the user. For example, you might set supportsPhoneCall to `1` for an item that represents a business, but not for an item that represents an academic paper that lists the phone numbers of the authors or the institution.

## See Also

### Supporting actions

var actionIdentifiers: [String]

The identifiers that specify custom actions the app supports for the item.

var supportsNavigation: NSNumber?

A value that indicates whether the item contains information sufficient to provide navigation to the location it represents.

var sharedItemContentType: UTType?

The file type of the item to enable the user to share items from Spotlight.

let CSActionIdentifier: String

A key that specifies the action’s identifier in a user activity.

