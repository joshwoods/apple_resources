

- UIKit
- UITableViewDiffableDataSourceReference
-  index(forSectionIdentifier:) 

Instance Method

# index(forSectionIdentifier:)

Returns an index for the section with the identifier you specify in the table view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func index(forSectionIdentifier identifier: Any) -> Int
```

## See Also

### Identifying sections

func sectionIdentifier(for: Int) -> Any?

Returns an identifier for the section at the index you specify in the table view.

