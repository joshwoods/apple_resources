

- UIKit
- UITableViewDiffableDataSource
-  sectionIdentifier(for:) 

Instance Method

# sectionIdentifier(for:)

Returns an identifier for the section at the index you specify in the table view.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
func sectionIdentifier(for index: Int) -> SectionIdentifierType?
```

## See Also

### Identifying sections

func index(for: SectionIdentifierType) -> Int?

Returns an index for the section with the identifier you specify in the table view.

