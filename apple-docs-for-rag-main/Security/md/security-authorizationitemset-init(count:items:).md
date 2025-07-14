

- Security
- AuthorizationItemSet
-  init(count:items:) 

Initializer

# init(count:items:)

Initializes an authorization item set with the given items.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    count: UInt32,
    items: UnsafeMutablePointer?
)
```

## Parameters 

`count`  

The number of items in the `items` array.

`items`  

A pointer to the first authorization item in an array of items.

