

- SwiftUI
- TabRole
-  search 

Type Property

# search

The search role.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var search: TabRole { get }
```

## Discussion

Searchable tab views will prefer to have the first tab with this role implement search. If no tabs are specified as the search tab, the tab view will apply search to all tabs, resetting search state as the selected tab changes.

