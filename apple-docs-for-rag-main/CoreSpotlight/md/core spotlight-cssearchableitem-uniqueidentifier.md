

- Core Spotlight
- CSSearchableItem
-  uniqueIdentifier 

Instance Property

# uniqueIdentifier

The value that uniquely identifies the searchable item within your app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var uniqueIdentifier: String { get set }
```

## Discussion

This property is required because it’s the only way to identify searchable items in the index when you need to access or delete them. When you create a searchable item, the system generates a UUID by default, but you can replace the default value with a unique identifier that makes sense in the context of your app. If you want to use a custom value for uniqueIdentifier, be sure to set it before the item is indexed for the first time.

## See Also

### Setting attributes on a searchable item

var domainIdentifier: String?

An optional identifier that represents the domain or owner of the item.

var attributeSet: CSSearchableItemAttributeSet

The set of attributes that contain metadata associated with the item in a CSSearchableItemAttributeSet object.

var expirationDate: Date!

The date after which the searchable item should no longer exist.

var isUpdate: Bool

A Boolean value that indicates whether to treat the item as an update instead of a new item.

