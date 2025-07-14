

- Core Spotlight
- CSSearchableItem
-  isUpdate 

Instance Property

# isUpdate

A Boolean value that indicates whether to treat the item as an update instead of a new item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var isUpdate: Bool { get set }
```

## Discussion

Set the value of this property to `true` if the item represents an update to information already in the index. Marking an item as an update makes the indexing process more efficient. If this property is `false` and the system encounters an item with the same identifier in the index, it deletes the old item and then inserts the new one. When the property is `true`, it updates the existing item, which saves time. If this property is `true` and the item doesn’t exist in the index, the system creates a new item.

When configuring the attributes for the item, set an attribute to `nil` to remove its value.

## See Also

### Setting attributes on a searchable item

var uniqueIdentifier: String

The value that uniquely identifies the searchable item within your app.

var domainIdentifier: String?

An optional identifier that represents the domain or owner of the item.

var attributeSet: CSSearchableItemAttributeSet

The set of attributes that contain metadata associated with the item in a CSSearchableItemAttributeSet object.

var expirationDate: Date!

The date after which the searchable item should no longer exist.

