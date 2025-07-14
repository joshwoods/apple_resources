

- ContactProvider
- ContactItemContentObserver
-  didEnumerate(\_:) 

Instance Method

# didEnumerate(\_:)

Provides an array of contact items to the observer.

iOS 18.0+iPadOS 18.0+

``` source
func didEnumerate(_: [ContactItem])
```

**Required**

## Discussion

You can call this method multiple times to fulfill the suggestedPageSize.

## See Also

### Providing contact items

enum ContactItem

An item in the contact database.

