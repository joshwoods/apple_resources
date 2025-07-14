

- Address Book
- ABRecord
-  uniqueId 

Instance Property

# uniqueId

Returns the unique ID for a record.

macOS

``` source
var uniqueId: String! { get }
```

## Return Value

The unique ID.

## Discussion

This method is equivalent to invoking value(forProperty:), passing `kABUIDProperty` as the argument.

## See Also

### Getting Identifying Information

var displayName: String!

A user-visible string representing the record.

