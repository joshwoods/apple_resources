

- AppKit
- NSDiffableDataSourceSnapshot
-  reloadSections(\_:) 

Instance Method

# reloadSections(\_:)

Reloads the data within the specified sections of the snapshot.

macOS 10.15.1+

``` source
mutating func reloadSections(_ identifiers: [SectionIdentifierType])
```

## Parameters 

`identifiers`  

The array of identifiers corresponding to the sections to reload in the snapshot.

## See Also

### Reloading Data

func reloadItems([ItemIdentifierType])

Reloads the data within the specified items in the snapshot.

