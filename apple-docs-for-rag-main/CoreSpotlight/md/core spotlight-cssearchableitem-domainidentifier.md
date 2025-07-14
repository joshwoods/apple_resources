

- Core Spotlight
- CSSearchableItem
-  domainIdentifier 

Instance Property

# domainIdentifier

An optional identifier that represents the domain or owner of the item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var domainIdentifier: String? { get set }
```

## Discussion

Specify a domain identifier to group items together and to make it easy to delete groups of items from the index. For example, you might specify an identifier for a mailbox in an account whose indexed data you want to remove when the account is deleted. In this example, domainIdentifier should be of the form `.`, where neither `` nor `` contain periods. To delete all items associated with the specified account and mailbox, you can call deleteSearchableItems(withDomainIdentifiers:completionHandler:) with a domainIdentifier of `.`. Or to delete all items associated with all mailboxes in the specified account, you can call deleteSearchableItems(withDomainIdentifiers:completionHandler:) with a domainIdentifier of ``.

## See Also

### Setting attributes on a searchable item

var uniqueIdentifier: String

The value that uniquely identifies the searchable item within your app.

var attributeSet: CSSearchableItemAttributeSet

The set of attributes that contain metadata associated with the item in a CSSearchableItemAttributeSet object.

var expirationDate: Date!

The date after which the searchable item should no longer exist.

var isUpdate: Bool

A Boolean value that indicates whether to treat the item as an update instead of a new item.

