

- UIKit
- UITableViewDiffableDataSourceReference
-  sectionIdentifier(for:) 

Instance Method

# sectionIdentifier(for:)

Returns an identifier for the section at the index you specify in the table view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func sectionIdentifier(for index: Int) -> Any?
```

## See Also

### Identifying sections

func index(forSectionIdentifier: Any) -> Int

Returns an index for the section with the identifier you specify in the table view.

