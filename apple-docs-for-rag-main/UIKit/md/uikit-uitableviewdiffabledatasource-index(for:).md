

- UIKit
- UITableViewDiffableDataSource
-  index(for:) 

Instance Method

# index(for:)

Returns an index for the section with the identifier you specify in the table view.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
func index(for sectionIdentifier: SectionIdentifierType) -> Int?
```

## See Also

### Identifying sections

func sectionIdentifier(for: Int) -> SectionIdentifierType?

Returns an identifier for the section at the index you specify in the table view.

