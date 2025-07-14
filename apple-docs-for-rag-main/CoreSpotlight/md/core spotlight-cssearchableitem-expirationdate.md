

- Core Spotlight
- CSSearchableItem
-  expirationDate 

Instance Property

# expirationDate

The date after which the searchable item should no longer exist.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var expirationDate: Date! { get set }
```

## Mentioned in 

Adding your app’s content to Spotlight indexes

## Discussion

If you don’t set the expirationDate property appropriately, the system automatically expires the item after a period of time.

## See Also

### Setting attributes on a searchable item

var uniqueIdentifier: String

The value that uniquely identifies the searchable item within your app.

var domainIdentifier: String?

An optional identifier that represents the domain or owner of the item.

var attributeSet: CSSearchableItemAttributeSet

The set of attributes that contain metadata associated with the item in a CSSearchableItemAttributeSet object.

var isUpdate: Bool

A Boolean value that indicates whether to treat the item as an update instead of a new item.

