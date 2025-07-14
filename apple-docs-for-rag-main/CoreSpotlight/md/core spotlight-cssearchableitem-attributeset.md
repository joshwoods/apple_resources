

- Core Spotlight
- CSSearchableItem
-  attributeSet 

Instance Property

# attributeSet

The set of attributes that contain metadata associated with the item in a CSSearchableItemAttributeSet object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var attributeSet: CSSearchableItemAttributeSet { get set }
```

## See Also

### Setting attributes on a searchable item

var uniqueIdentifier: String

The value that uniquely identifies the searchable item within your app.

var domainIdentifier: String?

An optional identifier that represents the domain or owner of the item.

var expirationDate: Date!

The date after which the searchable item should no longer exist.

var isUpdate: Bool

A Boolean value that indicates whether to treat the item as an update instead of a new item.

