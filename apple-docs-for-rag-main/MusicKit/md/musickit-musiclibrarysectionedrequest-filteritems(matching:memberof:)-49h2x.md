

- MusicKit
- MusicLibrarySectionedRequest
-  filterItems(matching:memberOf:) 

Instance Method

# filterItems(matching:memberOf:)

Filters items by a property for an array of possible values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func filterItems(
    matching keyPath: KeyPath,
    memberOf values: [Value]
) where Value : MusicLibraryRequestFilterValueMembershipComparable
```

