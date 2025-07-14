

- AppKit
- NSDiffableDataSourceSnapshotReference
-  reloadSections(withIdentifiers:) 

Instance Method

# reloadSections(withIdentifiers:)

Reloads the data within the specified sections of the snapshot.

macOS 10.15+

``` source
func reloadSections(withIdentifiers sectionIdentifiers: [Any])
```

## Parameters 

`sectionIdentifiers`  

The array of identifiers corresponding to the sections to reload in the snapshot.

## See Also

### Reloading data

func reloadItems(withIdentifiers: [Any])

Reloads the data within the specified items in the snapshot.

