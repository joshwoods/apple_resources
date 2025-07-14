

- AppKit
- NSDiffableDataSourceSnapshot
-  reloadItems(\_:) 

Instance Method

# reloadItems(\_:)

Reloads the data within the specified items in the snapshot.

macOS 10.15.1+

``` source
mutating func reloadItems(_ identifiers: [ItemIdentifierType])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the items to reload in the snapshot.

## See Also

### Reloading Data

func reloadSections([SectionIdentifierType])

Reloads the data within the specified sections of the snapshot.

