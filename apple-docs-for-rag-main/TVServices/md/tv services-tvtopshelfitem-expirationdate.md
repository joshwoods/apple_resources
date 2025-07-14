

- TV Services
- TVTopShelfItem
-  expirationDate 

Instance Property

# expirationDate

The date on which the item becomes unavailable.

tvOS 13.0+

``` source
var expirationDate: Date? { get set }
```

## Discussion

Specify an expiration date when the content associated with the item has a limited lifespan. For example, use it to specify the date on which a rented movie expires. The system uses this property to remove items that have expired since you last provided data.

## See Also

### Getting the Item Attributes

var identifier: String

The unique identifier for the item.

