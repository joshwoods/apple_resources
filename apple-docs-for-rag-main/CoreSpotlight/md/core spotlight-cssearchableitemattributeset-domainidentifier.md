

- Core Spotlight
- CSSearchableItemAttributeSet
-  domainIdentifier 

Instance Property

# domainIdentifier

An identifier that represents the domain or owner of the item.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var domainIdentifier: String? { get set }
```

## Discussion

Specify a domain identifier to group items together and to make it easy to delete groups of items from the index. For example, to delete a user activity, you can set this property on the contentAttributeSet property of the NSUserActivity object and then call deleteSearchableItems(withDomainIdentifiers:completionHandler:) on the default().

## See Also

### Describing general attributes

var alternateNames: [String]?

An array of localized strings that represent alternate display names for the item.

var contentType: String?

The uniform type identifier (UTI) of the item.

var contentTypeTree: [String]?

An attribute type that identifies a custom hierarchy of types to describe the attributes of your item.

var contentURL: URL?

The file URL of the content to index.

var darkThumbnailURL: URL?

The local file URL of the thumbnail image for the item when Dark Mode is active.

var displayName: String?

A localized string that contains the name of the item, suitable to display in the user interface.

var keywords: [String]?

An array of keywords associated with the item, such as work, birthday, important, and so on.

var metadataModificationDate: Date?

The date on which the last metadata attribute was changed.

var path: String?

The complete path to the item.

var rankingHint: NSNumber?

A number that indicates the relative importance of the item among other items from the app.

var relatedUniqueIdentifier: String?

The unique identifier for the item to which the activity is related.

var thumbnailData: Data?

Image data that represents the thumbnail of the item.

var thumbnailURL: URL?

The local file URL of the thumbnail image for the item.

var title: String?

The title of the item.

var weakRelatedUniqueIdentifier: String?

The unique identifier for the item to which the activity is related, but not linked.

